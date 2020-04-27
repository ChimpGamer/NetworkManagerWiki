# CommandBlocker

The CommandBlocker module uses regex to check if a player uses a blocked command.

With regex you can make efficient rules to block commands. For example:

```text
^/(op\b|bukkit:op|minecrafft:op) #This blocks /op /bukkit:op and /minecraft:op
/(whitelist|bukkit:whitelist|minecraf:whitelist) #This blocks /whitelist /bukkit:whitelist and /minecraft:whitelist
^/(rl\b|reload) #This blocks /rl and /reload

If you want to block just a single command you can use ^/<command>\b
Example: ^/kill\b #This blocks /kill but not /killall

If you want to block /? for example you can use \/\?

Want to block all commands that contain a : ? No problem!
Just use [:] and it will block commands like bukkit:about and bukkit:plugins
```

You can test your regex expressions at an online website like: [https://regexr.com/](https://regexr.com/)

Want to share your regex expressions? Send me a messages on spigot or discord and I'll add them to this page with your name and explanation.

### Permissions

**Permission**: networkmanager.commandblocker.bypass  
Allows you to bypass all blocked commands specified in the NetworkManager CommandBlocker

**Permission**: networkmanager.commandblocker.bypass.&lt;command&gt;  
Allows you to bypass a specific blocked command



