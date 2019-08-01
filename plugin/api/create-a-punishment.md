# Create a punishment

```java
package nl.chimpgamer.networkmanager.example;

import nl.chimpgamer.networkmanager.common.modules.punishments.NMPunishment;
import nl.chimpgamer.networkmanagerapi.NetworkManagerPlugin;
import nl.chimpgamer.networkmanagerapi.modules.player.Player;
import nl.chimpgamer.networkmanagerapi.modules.punishments.Punishment;

import java.util.Optional;

public class Example {
    private final NetworkManagerPlugin networkManager;
    
    public Example(NetworkManagerPlugin networkManager) {
        this.networkManager = networkManager;
    }
    
    public void createPunishment() {
        Optional<Player> opPlayer = this.getNetworkManager().getPlayerSafe("UUID of player that you want to punish here");
        if (!opPlayer.isPresent()) {
            getNetworkManager().debug("Could not fetch player from database!");
            return;
        }
        Player player = opPlayer.get();
        int id = this.getNetworkManager().getCacheManager().getCachedPunishments().getLatestID();
        Punishment punishment = new NMPunishment(this.getNetworkManager(), id, Punishment.Type.GBAN, player.getUuid(), "uuid of punisher", null, System.currentTimeMillis(), -1, "IP of player that you punish", null, "Punishment reason here", true);
        punishment.punish();
        player.notify(player.generateBanMessage(punishment), punishment.getType());
    }
    
    private NetworkManagerPlugin getNetworkManager() {
        return networkManager;
    }
}
```

