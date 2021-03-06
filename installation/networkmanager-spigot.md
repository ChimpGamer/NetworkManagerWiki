# NetworkManager \(Spigot\)

### Requirements

1. Make sure you have Java 8 installed!​
2. Make sure NetworkManager \(BungeeCord\) is successfully configured and working.
3. Make sure you have set in your spigot.yml bungeecord: true

### Features

1. Permission system on spigot \(can hook into vault if enabled\).
2. Placeholders, you can download the plugins here: [PlaceholderAPI ](https://www.spigotmc.org/resources/placeholderapi.6245/)& [MVdWPlaceholdersAPI](https://www.spigotmc.org/resources/mvdwplaceholderapi.11182/)
3. Proxy Only
4. Extensions on spigot like: SimpleChat & Tags
5. When using the ignore command it will actually ignore players that are ignored in the chat.

### Installation

1. Drop the plugin \(NetworkManager\) in your Spigot plugins folder.
2. Start your Spigot server.
3. Open the settings.yml located at /plugins/NetworkManager/settings.yml.
4. Enter your MySQL host, port, username, password and database.
5. \(Optional\) Enable Redis. Enter redis host and password if you set one.
6. If you use the permission system maken sure you set the correct servername in the settings.yml.
7. Restart your Spigot server and it should work without issues.

### Common issues

1. If you see something like this: "Could not create connection to database server. Attempted reconnect 3 times. Giving up." it means it couldn't connect to your MySQL database. Check in the setting.yml if you have set the correct settings.

