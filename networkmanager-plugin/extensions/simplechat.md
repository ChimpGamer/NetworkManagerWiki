# SimpleChat

This is the default settings.yml. In this file you can create as much formats as you want. To allow a player to use a format you'll have to give them the permission: simplechat.format.\<formatName>.

| Permission                          | Description                                                                            |
| ----------------------------------- | -------------------------------------------------------------------------------------- |
| simplechat.format.\<formatName>     | Gives the player permission to use this format                                         |
| simplechat.chatcolor                | Gives the permission to use colorcodes. \&e                                            |
| simplechat.showitem                 | Gives the permission to use the itemkeywords. def: \[item]                             |
| simplechat.chatlinks                | Gives the player permission to send **clickable** url links                            |
| simplechat.playermention            | Gives the player permission to tag other players                                       |
| simplechat.bypass.move              | Gives the player permission to bypass the move before chat protection                  |
| simplechat.customkeyword.\<keyword> | Gives the player permission to use a customkeyword that is defined in the settings.yml |

You can reload the settings.yml with /nmb extensions reloadconfig SimpleChat

The options pretty much explain themselves.

**Note: To use placeholderapi placeholders, use \<papi:"placeholder\_name">**

{% hint style="info" %}
ItemKeywords only work with paper 1.16.3 and newer!
{% endhint %}

{% code title="settings.yml" %}
```yaml
crossServerChat: false
blockChatUntilMoved: true

itemKeywords:
  - '[item]'
  - '{item}'

customKeywords:
  '[pos]': '<gold>World: <white><player_world> <gold>X:<white><player_x> <gold>Y:<white><player_y> <gold>Z:<white><player_z>'
  '[ping]': '<player_colored_ping> ms'

playerMention:
  enabled: false
  color: '<green>'

formats:
  default:
    messageFormat: '<dark_gray>[<prefix><dark_gray>] <hover:show_text:"<red><yellow>Example tooltip"><displayname_with_click></hover> <dark_gray><arrow_right> <gray><message>'
    priority: 100
    
placeholders:
  displayname_with_click: '<click:suggest_command:"/msg <playername> "><yellow><displayname></click>'
  arrow_right: »
  arrow_left: «
```
{% endcode %}

## How to install?

1. [Download ](https://discord.com/channels/222070253172031500/564936267037540353)the extension from the Discord server.
2. Drop the extension jar in the extensions folder on your spigot server.
3. Restart your spigot server.

