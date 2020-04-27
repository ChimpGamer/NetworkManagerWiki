# Tags

### Requirements

1. The NetworkManager plugin installed and configured on your spigot server.
2. A Permission system.
3. PlaceholderAPI or MVdWPlaceholderAPI Installed \(If you are gonna use it in a Scoreboard, Tab or Other chat plugin\).
4. \(Optional\) If you want to use tags in chat you need a chat plugin that supports PlaceholderAPI or MVdWPlaceholderAPI \(You can also just use the tags in a scoreboard plugin or so\).

### Installation

1. Download the extension from the Discord server.
2. Drop the extension jar in the extensions folder on your Bukkit server.
3. Restart your Bukkit server.
4. Enable the tags module \(module\_tags\).
5. Create some tags in the Web Interface or with the command.
6. Assign the permissions `(networkmanager.tags.<Tagname>)`.
7. Put the correct placeholder in your Chat plugin \(PAPI: %networkmanager\_tag%, MVdW: {networkmanager\_tag}\).

### Commands

`/tags (Page) - Opens the Tags GUI (permission: networkmanager.tags.gui)`  
`/tags create <Tagname> <Tag> (Server) (permission: networkmanager.tags.create)`  
`/tags delete <Tagname> (permission: networkmanager.tags.delete)`  
`/tags setdesc <Tagname> <Description> (permission: networkmanager.tags.setdescription)`  
`/tags set <Username> <Tagname> (permission: networkmanager.tags.set)`  
`/tags unset/clear <Username> (permission: networkmanager.tags.unset)`  
`/tags permission <Tagname/TagId> (permission: networkmanager.tags.permission)`

The server parameter can be replaced with "all" to indicate a global setting. Parameters within \(\)'s are optional parameters. Parameters within &lt;&gt;'s are required.

### Tips

1. In the description the placeholder %newline% is allowed and will create a new line in the Description.

