# SimpleChat

This is the default settings.yml. In this file you can create as much formats as you want. To allow a player to use a format you'll have to give them the permission: simplechat.format.&lt;formatName&gt;.

| Permission | Description |
| :--- | :--- |
| simplechat.format.&lt;formatName&gt; | Gives the player permission to use this format |
| simplechat.chatcolor | Gives the permission to use colorcodes. &e |
| simplechat.showitem | Gives the permission to use the itemkeywords. def: \[item\] |

You can reload the settings.yml with /nmb extensions reloadconfig SimpleChat

The options pretty much explain themselves.

{% hint style="info" %}
ItemKeywords only work with paper 1.16.3 and newer!
{% endhint %}

{% code title="settings.yml" %}
```yaml
crossServerChat: false

itemKeywords:
  - '[item]'
  - '{item}'

formats:
  default:
    prefix: '&8[%prefix%&8] '
    name: '%username%'
    suffix: ' &8» '
    chatColor: '&7'
    prefixTooltip: []
    nameTooltip:
    - '&eExample tooltip of &6%playername%'
    suffixTooltip: []
    prefixClickCommand: ''
    nameClickCommand: ''
    suffixClickCommand: ''
    priority: 100
```
{% endcode %}

## How to install?

1. [Download ](https://discordapp.com/channels/222070253172031500/564936267037540353/790638738828558356)the extension from the Discord server.
2. Drop the extension jar in the extensions folder on your spigot server.
3. Restart your spigot server.

