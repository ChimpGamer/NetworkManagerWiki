# Hook into the API

## Classes:

{% code title="MainClass.java" %}
```java
package example.main;

import org.bukkit.plugin.java.JavaPlugin;

import example.api.NetworkManagerAPIHook;

public class MainClass extends JavaPlugin {
	private final NetworkManagerAPIHook nmApiHook;
	
	public void onEnable() {
		if (this.getServer().getPluginManager().getPlugin("NetworkManager") != null) {
			this.nmApiHook = new NetworkManagerAPIHook(this);
        }
	}
	
	public void onDisable() {
		this.nmApiHook = null;
	}
	
	public NetworkManagerAPIHook getNMApiHook() {
        return this.nmApiHook ;
    }
}
```
{% endcode %}

{% code title="NetworkManagerAPIHook.java" %}
```java
package example.nmapi;
 
import java.util.List;
import java.util.Optional;
import java.util.UUID;

import org.bukkit.plugin.Plugin;

import example.main.YourMainClass;
import nl.chimpgamer.networkmanager.api.NetworkManagerPlugin;
import nl.chimpgamer.networkmanager.api.cache.CacheManager;
import nl.chimpgamer.networkmanager.api.models.permissions.Group;
import nl.chimpgamer.networkmanager.api.models.permissions.PermissionPlayer;
import nl.chimpgamer.networkmanager.api.models.player.Player;
 
public class NetworkManagerAPIHook {
    private NetworkManagerPlugin networkManager;
 
    public NetworkManagerAPIHook(YourMainClass yourMainClass) {
        Plugin plugin = mainClass.getServer().getPluginManager().getPlugin("NetworkManager");
        if (plugin != null) {
            networkManager = (NetworkManagerPlugin) plugin;
			yourMainClass.getLogger().info("Hooked into NetworkManager");
        }
    }
    
    /**
     * Get the NetworkManager CacheManager.
     * @return The NetworkManager CacheManager.
	 */
    public CacheManager getCacheManager() {
        return networkManager.getCacheManager();
    }
    
    /**
     * Get NetworkManager Player.
     * @param uuid UUID of the player.
     * @return an optional {@link Player} object
	 */
    public Optional<Player> getPlayer(UUID uuid) {
        return getCacheManager().getCachedPlayers().getPlayerSafe(uuid);
    }
 
    /**
     * Get an NetworkManager Cached player.
     * @param username The username of the player.
     * @return an optional {@link Player} object */
    public Optional<Player> getPlayer(String username) {
        return getCacheManager().getCachedPlayers().getPlayerSafe(username);
    }
 
    /**
	 * Get an player permission from NetworkManager.
	 * @return The NetworkManager Cached player permission.
	 * @param uuid UUID of the player.
	 * @author ChimpGamer
     * @since 2.5.0
	 */
    public PermissionPlayer getPermissionsPlayer(UUID uuid) {
        return networkManager.getPermissionManager().getPermissionPlayer(uuid);
    }
 
    /**
	 * Get the NetworkManager Cached player groups.
	 * @return The NetworkManager Cached player groups.
	 * @param uuid UUID of the player.
	 */
    public List<Group> getPlayerGroups(UUID uuid) {
        return getPermissionsPlayer(uuid).getGroups();
    }
}
```
{% endcode %}

