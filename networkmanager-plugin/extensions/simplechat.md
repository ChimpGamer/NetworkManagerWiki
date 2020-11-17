# SimpleChat

This is the default settings.yml. In this file you can create as much formats as you want. To allow a player to use a format you'll have to give them the permission: simplechat.format.&lt;formatName&gt;.

You can reload the settings.yml with /nmb extensions reloadconfig SimpleChat

The options pretty much explain themselves.

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

