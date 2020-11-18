# PlayerNameList

This is the default formats.yml. In this file you can create as much formats as you want. To allow a player to use a format you'll have to give them the permission: playernamelist.format.&lt;formatName&gt;.

You can reload the formats.yml with /nmb extensions reloadconfig PlayerNameList

The options pretty much explain themselves.

```yaml
updateInterval: 10 # In seconds

formats:
  default:
    prefix: '%prefix% '
    name: '&e%playername%'
    suffix: ' %suffix%'
    priority: 100
```

