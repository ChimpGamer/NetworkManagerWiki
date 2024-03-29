# Tags

Allow players the to select a tag that can be displayed in the chat or anywhere you want if they have permission for it.

### Requirements

1. The NetworkManager plugin installed and configured on your spigot server.
2. A Permission system.
3. PlaceholderAPI Installed (If you are gonna use it in a Scoreboard, Tab or Other chat plugin, SimpleChat is supported by default: \<tag>).

### Installation

1. [Download ](https://discord.com/channels/222070253172031500/1102241984581750835)the extension from the Discord server.
2. Drop the extension jar in the extensions folder on your Bukkit server.
3. Restart your Bukkit server.
4. Enable the tags module (module\_tags).
5. Create some tags in the Web Interface or with the command.
6. Assign the permissions `(networkmanager.tags.<Tagname>)`.
7. Put the correct placeholder in your Chat plugin (PAPI: %networkmanager\_tag%, MVdW: {networkmanager\_tag}).

### Commands

`/tags (page)` \
**Permission**: networkmanager.tags.gui\
Opens the Tags GUI

`/tags create [tagName] [tag] (server)` \
**Permission**: networkmanager.tags.create\
Create a tag with the specified arguments

`/tags delete [tagName]` \
**Permission**: networkmanager.tags.delete\
Delete a tag

`/tags setdesc [tagName] [description]` \
**Permission**: networkmanager.tags.setdescription\
Set the description for a tag

`/tags set [userName] [tagName]` \
**Permission**: networkmanager.tags.set\
Set the tag for a player

`/tags unset/clear [userName]` \
**Permission**: networkmanager.tags.set\
Remove the current tag from a player

`/tags permission [tagName/tagId]` \
**Permission**: networkmanager.tags.permission\
Get the permission of a tag

`/tags reload (tagId)` \
**Permission**: networkmanager.tags.reload\
Reload tag(s)

The server parameter can be replaced with "all" to indicate a global setting. Parameters within ()'s are optional parameters. Parameters within \[]'s are required.

### Tips

1. In the description the placeholder %newline% is allowed and will create a new line in the Description.
2. You can force tags on players using the networkmanager.tags.forcetag.\<tag> permission.
