# Create a punishment

```java
package nl.chimpgamer.networkmanager.example;

import nl.chimpgamer.networkmanager.common.modules.punishments.NMPunishment;
import nl.chimpgamer.networkmanagerapi.NetworkManagerPlugin;
import nl.chimpgamer.networkmanagerapi.models.player.Player;
import nl.chimpgamer.networkmanagerapi.models.punishments.Punishment;

import java.util.Optional;

public class Example {
    private final NetworkManagerPlugin networkManager;
    
    public Example(NetworkManagerPlugin networkManager) {
        this.networkManager = networkManager;
    }
    
public void createPunishment(Player player) {
        final CachedPunishments cachedPunishments = this.getNetworkManager().getCacheManager().getCachedPunishments();
        Punishment.Builder punishmentBuilder = cachedPunishments.createPunishmentBuilder();
        Punishment punishment = punishmentBuilder
                .setType(Punishment.Type.GBAN)
                .setUuid(UUID.fromString("uuid-here"))
                .setPunisher(UUID.fromString("uuid-of-punisher-here"))
                .setTime(System.currentTimeMillis())
                .setReason("Just a simple reason here.")
                .build();
        punishment.punish();
        
        player.executePunishmentActions(punishment);
    }
    
    private NetworkManagerPlugin getNetworkManager() {
        return networkManager;
    }
}
```

