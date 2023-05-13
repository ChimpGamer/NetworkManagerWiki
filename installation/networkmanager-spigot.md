# NetworkManager (Spigot)

### Requirements

1. Make sure you have Java 8, 11, 16 or 17 installed!​
2. Make sure NetworkManager (BungeeCord) is successfully configured and working.
3. Make sure you have set in your spigot.yml bungeecord: true

### Features

1. Permission system on spigot (can hook into vault if enabled).
2. PlaceholderAPI support. You can download the plugin here: [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/)
3. Proxy Only
4. Extensions on spigot like: SimpleChat & Tags (you can download them in the discord server)
5. Ignore feature will work with most chat plugins.

### Installation

1. Download the jar from (Discord) [here](https://discord.com/channels/222070253172031500/1094976129045114960).
2. Drop the plugin (NetworkManager) in your Spigot plugins folder.
3. Start your Spigot server.
4. Open the settings.yml located at /plugins/NetworkManager/settings.yml.
5. Enter your MySQL host, port, username, password and database.
6. (Optional) Enable Redis. Enter redis host and password if you set one.
7. If you use the permission system maken sure you set the correct servername in the settings.yml.
8. Restart your Spigot server and it should work without issues.

### Common issues

1. If you see something like this: "Could not create connection to database server. Attempted reconnect 3 times. Giving up." it means it couldn't connect to your MySQL database. Check in the setting.yml if you have set the correct settings.
