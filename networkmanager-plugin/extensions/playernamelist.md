# PlayerListName

This is the default formats.yml. In this file you can create as much formats as you want. To allow a player to use a format you'll have to give them the permission: playernamelist.format.\<formatName>.

You can reload the formats.yml with /nmb extensions reloadconfig PlayerListName

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

## How to install?

1. Download the extension from [github](https://github.com/ChimpGamer/PlayerListName-Extension).
2. Drop the extension jar in the extensions folder on your spigot/paper server.
3. Restart your spigot/paper server.
4. Configure the formats.yml to your liking.
5. Reload the configs with /nmb extensions reloadconf PlayerListName

## FAQ about this extension

{% hint style="info" %}
How can I adjust the order in the PlayerNameList extension?

You can't. Use NameTagEdit or a similar plugin. This is just a simple extension that allows you to change the name of your players in the TAB.
{% endhint %}
