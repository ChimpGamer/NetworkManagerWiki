# Placeholders

**Note: This list is updated for NetworkManager 2.8.0**

### General Placeholders

| Placeholder | Description |
| :--- | :--- |
| %newline% | Will create a new line in a string. |
| %pluginprefix% | Returns the plugin prefix which can be configured in the languages |
| %uniquejoins% | Returns the amount of unique joins on the server. |
| %onlineplayers% | Returns the amount of online players. |
| %maxplayers% | Returns the amount of max allowed players on the server. |
| %message\_&lt;messageKey&gt;% | Returns the messages from the message key defined. Example: %message\_lang\_time\_year% would return Year if the selected language is English. |
| %randomplayer\_&lt;x&gt;% | Returns a list of random online players. Where the x is you define the amount of random players. |
| %players\_&lt;server/servergroup&gt;% | Returns the amount of online players on the defined server or servergroup. |

### General Placeholders \(Player Online\)

| Placeholder | Description |
| :--- | :--- |
| %playername% | Returns the name of the player |
| %username% | Returns the username of the player. If the player has a name color this will apply. |
| %nickname% | Returns the nickname of the player. If the player has no nickname it will return the username. |
| %server% | Returns the name of the server the player is currently playing on. |
| %version% | Returns the client version of the player. |
| %country% | Returns the country code of the detected country. |
| %ip% | Returns the ip of the player. |
| %status% | Returns the status of the player. Online or Offline. Result configurable lang\_online and lang\_offline. |
| %playtime% | Returns the playtime of the player. |
| %liveplaytime% | Returns the live playtime of the player. \(This placeholder will automatically calculate the playtime when requested\). |
| %playtime\_h% | Returns the playtime in hours. |
| %playtime\_m% | Returns the playtime in minutes. |
| %playtime\_s% | Returns the playtime in seconds. |
| %liveplaytime\_h% | Returns the live playtime in hours. |
| %liveplaytime\_m% | Returns the live playtime in minutes. |
| %liveplaytime\_s% | Returns the live playtime in seconds. |
| %namecolor% | Returns the name color if the player has one. |
| %language% | Returns the name of the selected language. |
| %ping% | Returns the ping in ms of the player. |
| %serverplayers% | Returns the amount of online players of the server the player is currently playing on. |

### Punishment Placeholders

| Placeholder | Description |
| :--- | :--- |
| %id% | Returns the id of the punishment |
| %type% | Returns the name of the punishment type |
| %uuid% | Returns the UUID of the player that got punished |
| %playername% | Returns the name of the player that got punished |
| %punisher% | Returns the name of the punisher. That could either be Console or a playername |
| %time% | Returns the date and time of the start of the punishment. Format can be configured by changing lang\_punishment\_datetime\_format |
| %ends% | Returns the date and time of the ending of the punishment. Format can be configured by changing lang\_punishment\_datetime\_format |
| %expires% | Returns in years, months, weeks, days, hours, minutes, seconds how long the punishment will remain active. |
| %server% | Returns the name of the server where the player was banned from. If it is a global ban it will simply return Global. |
| %reason% | Returns the reason of the punishments. |
| %unbanner% | Returns the name of the unbanner if the player got unbanned by console or staff. |

### Motd Placeholders

| Placeholder | Description |
| :--- | :--- |
| %date% | Returns the current date. Can be changed by changing lang\_date\_format |

