# SimpleChat

This is the default formats.yml. In this file you can create as much formats as you want. To allow a player to use a format you'll have to give them the permission: simplechat.format.&lt;formatName&gt;.

You can reload the formats.yml with /nmb extensions reloadconfig SimpleChat

The options pretty much explain themselves.

{% tabs %}
{% tab title="formats.yml" %}
```yaml
crossServerChat: false

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
```
{% endtab %}
{% endtabs %}

