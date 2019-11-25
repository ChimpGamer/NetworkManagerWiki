# Get the language as an string.

!!! Example is for spigot only !!!

{% code title="LanguageName.java" %}
```java
package example.nmapi;

import java.util.Optional;
import java.util.UUID;

import org.bukkit.command.CommandSender;

import example.main.MainClass;
import nl.chimpgamer.networkmanager.api.exceptions.LanguageNotFoundException;
import nl.chimpgamer.networkmanager.api.models.player.Player;

public class LanguageName {
	
	private NetworkManagerAPIHook nmapi;
     
    public LanguageName(MainClass mainClass) {
        this.nmapi = mainClass.getNmbApi();
    }
    
    /**
     * Get the languagename from NetworkManager.
     * @param sender The person that you need the language from.
     * @return The language name.
     * @author Daniel Markink and ChimpGamer
	 */
    public String getLanguageName(CommandSender sender) {
        final CachedValues cachedValues = this.getNmapi().getCacheManager().getCachedValues();
        final CachedLanguages cachedLanguages = this.getNmapi().getCacheManager().getCachedLanguages();
        final CachedPlayers cachedPlayers = this.getNmapi().getCacheManager().getCachedPlayers();
        if (!(sender instanceof org.bukkit.entity.Player)) {
            return cachedValues.getString(Setting.LANGUAGE_DEFAULT) != null ? cachedValues.getString(Setting.LANGUAGE_DEFAULT) : "English";
        }
        UUID uuid = ((org.bukkit.entity.Player) sender).getUniqueId();
        Optional<Player> opPlayer = cachedPlayers.getPlayerSafe(uuid);
        try {
            if (opPlayer.isPresent()) {
                Player player = opPlayer.get();
                Language language = cachedLanguages.getLanguage(player.getLanguage());
                return language != null ? language.getName() : (cachedValues.getString(Setting.LANGUAGE_DEFAULT) != null ? cachedValues.getString(Setting.LANGUAGE_DEFAULT) : "English");
            } else {
                return cachedValues.getString(Setting.LANGUAGE_DEFAULT) != null ? cachedValues.getString(Setting.LANGUAGE_DEFAULT) : "English";
            }
        } catch (LanguageNotFoundException ex) {
            ex.printStackTrace();
            return cachedValues.getString(Setting.LANGUAGE_DEFAULT) != null ? cachedValues.getString(Setting.LANGUAGE_DEFAULT) : "English";
        }
    }
    
    private NetworkManagerAPIHook getNmapi() {
        return nmapi;
    }
}

```
{% endcode %}

