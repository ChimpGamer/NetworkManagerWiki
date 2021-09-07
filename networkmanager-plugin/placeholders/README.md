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
| %randomplayer@&lt;x&gt;% | Returns a list of random online players. Where the x is you define the amount of random players. Example: %randomplayer@5% |
| %players@&lt;server/servergroup&gt;% | Returns the amount of online players on the defined server or servergroup. Example: %players@lobby% |

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
| {newline} | Incase %newline% breaks the motd when using % as in 50% off or something you can use this |

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Server Placeholders

| Placeholder | Description |
| :--- | :--- |
| %newline% | Will create a new line in a string. |
| %date% | Returns the current date. Format can be changed by changing lang\_date\_format |
| %pluginprefix% | Returns the plugin prefix which can be configured in the languages |
| %servername% | Returns the name of the server. \(For BungeeCord it will return BungeeCord. For Spigot server it depends on your configuration\) |
| %uniquejoins% | Returns the amount of unique joins on the server. |
| %onlineplayers% | Returns the amount of online players |
| %total\_punishments% | Returns the total amount of executed punishments |
| %total\_reports% | Returns the total amount of reports created. |
| %total\_tickets% | Returns the total amount of tickets created. |
| %closed\_tickets% | Returns the amount of closed tickets. |
| %open\_tickets% | Returns the amount of open tickets. |
| %message\_&lt;messageKey&gt;% | Returns the messages from the message key defined. Example: %message\_lang\_time\_year% would return Year if the selected language is English. |
| %countdown\_24-12-2021% | Returns a countdown from current date until the specified date. The format of the date depends on your setting lang\_date\_format for the English Language. |
| %countdown-dd-MM-yyyy\_24-12-2021% | Returns a countdown from current date until the specified date. The format can be specified in this placeholder. |

-- BungeeCord Only --

| Placeholder | Description |
| :--- | :--- |
| %maxplayers% | Returns the amount of max allowed players on the network. |
| %randomplayer@&lt;x&gt;% | Returns a list of random online players. Where the x is you define the amount of random players. Example: %randomplayer@5% |
| %players@&lt;server/servergroup&gt;% | Returns the amount of online players on the defined server or servergroup. Example: %players@lobby% |
| %serverplayers% | Only when player is available. |

### Player Placeholders

| Placeholder | Description |
| :--- | :--- |
| %uuid% |  |
| %playername% |  |
| %username% |  |
| %displayname% |  |
| %nickname% |  |
| %namecolor |  |
| %server% |  |
| %version% |  |
| %country |  |
| %ip% |  |
| %status% |  |
| %playtime% |  |
| %liveplaytime% |  |
| %playtime\_h% |  |
| %playtime\_m% |  |
| %playtime\_s% |  |
| %liveplaytime\_h% |  |
| %liveplaytime\_m% |  |
| %liveplaytime\_s% |  |
| %language% |  |
| %tag% |  |
| %ping% |  |

### Permission Placeholders

| Placeholder |  |
| :--- | :--- |
| %ownprefix% |  |
| %ownsuffix% |  |
| %prefix% |  |
| %suffix% |  |
| %ownprefix\_color% |  |
| %ownsuffix\_color% |  |
| %prefix\_color% |  |
| %suffix\_color% |  |
| %primarygroup% |  |
| %prefix\_&lt;ladder&gt;% |  |
| %firstprefix\_&lt;ladders&gt;% |  |
| %suffix\_&lt;ladder&gt;% |  |
| %firstsuffix\_&lt;ladders&gt;% |  |
| %groupname\_&lt;ladder&gt;% |  |
| %firstgroup\_&lt;ladder&gt;% |  |
| %permexpirytime\_&lt;permission&gt;% |  |
| %permexpirydate\_&lt;permission&gt;% |  |
| %ownpermexpirytime\_&lt;permission&gt;% |  |
| %ownpermexpirydate\_&lt;permission&gt;% |  |
| %groupexpirytime\_&lt;permission&gt;% |  |
| %groupexpirydate\_&lt;permission&gt;% |  |
| %group\_&lt;groupname&gt;\_id% |  |
| %group\_&lt;groupname&gt;\_ladder% |  |
| %group\_&lt;groupname&gt;\_rank% |  |
| %group\_&lt;groupname&gt;\_prefix% |  |
| %group\_&lt;groupname&gt;\_suffix% |  |
| %group\_&lt;groupname&gt;\_permexpiretime\_&lt;permission&gt;% |  |
| %group\_&lt;groupname&gt;\_permexpiredate\_&lt;permission&gt;% |  |
| %group\_&lt;groupname&gt;\_prefix\_&lt;server&gt;% |  |
| %group\_&lt;groupname&gt;\_suffix\_&lt;server&gt;% |  |

