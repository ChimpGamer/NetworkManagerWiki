# Get the language as an string.

{% code-tabs %}
{% code-tabs-item title="LanguageName.java" %}
```java
package example.nmapi;

import java.util.Optional;
import java.util.UUID;

import org.bukkit.command.CommandSender;

import example.main.MainClass;
import nl.chimpgamer.networkmanagerapi.exceptions.LanguageNotFoundException;
import nl.chimpgamer.networkmanagerapi.modules.player.Player;

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
		if(!(sender instanceof org.bukkit.entity.Player)) {
            if (this.nmapi.getCacheManager().getCachedValues().getValues().containsKey("setting_language_default")) {
                return this.nmapi.getCacheManager().getCachedValues().getString("setting_language_default");
            } else {
            	// Fallback language name if the language can not be retrieved.
                return "English";
            }
		} else {
			UUID uuid = ((org.bukkit.entity.Player) sender).getUniqueId();
			Optional<Player> nmbplayer = this.nmapi.getCacheManager().getCachedPlayers().getPlayerSafe(uuid);
			try {
				if(nmbplayer.isPresent()) {
					return this.nmapi.getCacheManager().getCachedLanguages().getLanguage(nmbplayer.get().getLanguage()).getName();
				} else {
					if (this.nmapi.getCacheManager().getCachedValues().getValues().containsKey("setting_language_default")) {
		                return this.nmapi.getCacheManager().getCachedValues().getString("setting_language_default");
		            } else {
						// Fallback language name if the language can not be retrieved.
		                return "English";
		            }
				}
			} catch (LanguageNotFoundException e) {
				e.printStackTrace();
				if (this.nmapi.getCacheManager().getCachedValues().getValues().containsKey("setting_language_default")) {
	                return this.nmapi.getCacheManager().getCachedValues().getString("setting_language_default");
	            } else {
					// Fallback language name if the language can not be retrieved.
	                return "English";
	            }
			}
        }
    }
}

```
{% endcode-tabs-item %}
{% endcode-tabs %}

