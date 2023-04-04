# ServerManager

## What can you do with ServerManager?

With ServerManager you can add, remove, modify and more like you would do in the BungeeCord config (without restarting the server) but with more options, settings and features. You can also create servergroups to balance the players.

## Requirements

The ServerManager requires only 1 thing. You need at least one server in your BungeeCord configuration. It is recommended that you put your authentication or hub/lobby servers in there as fallback of the ServerManager system.

Also make sure you disable \`force\_default\_server\` in the config.yml of BungeeCord otherwise you will get this error on login: [https://pastebin.com/3RQxi1N1](https://pastebin.com/3RQxi1N1)

## How to add a server

1. Go to the Web interface and click on Servers.
2. Click Add Server.
3. Fill in the Form (Servername, IP and Port everything else is optional). NOTE: BungeeCord doesn't like spaces in the ServerName so don't use spaces or it will cause problems.
4. (Optional) If you want to only allow some versions on a specific servers you can enter something like "1.8, 1.12.1, 1.12.2" (Only allows all 1.8 clients, 1.12.1 and 1.12.2 clients) in Allowed Versions.
5. Click create and the Server will be added.
6. Run the command /servermanager reload (servername) to apply the changes. WARNING: This can mess up things if there are still players playing on the server you reloaded!

## How to edit a server

1. Go to the Web interface and click on Servers.
2. Click on the orange edit icon.
3. Change a setting.
4. Press save when you're done.
5. Run the command /servermanager reload (servername) to apply the changes. WARNING: This can mess up things if there are still players playing on the server you reloaded!

## How to create a servergroup

1. Go to the Web interface and click on Servers.
2. Click Create ServerGroup.
3. Fill in the Form. Groupname is the name of the group. lobbies for example. ServerIds are the Id's of your Servers. You can find them in the Servers list. You need to enter server id's like "1,3,6,9,12" (Without quotes).
4. Click create and the servergroup will be added.

## How to add servers to a servergroup

1. Go to the Web interface and click on Servers.
2. Click on the name a servergroup.
3. Click Add Server.
4. Fill in the Server Name or Server Id.
5. Click Add

## Forced Hosts

Let's say you have some bedwars servers and bedwars game lobbies and you want to use forced hosts to play bedwars without joining the main lobbies first. If you've created a group with bedwars lobbies you can easily do that using the forced\_hosts setting in the config.yml of BungeeCord like this:

```yaml
  forced_hosts:
    bedwars.yourdomain.com: bedwars_lobbies # <- bedwars_lobbies in the groupname I used in this example
```

You can also do this for single servers liked you're used to of course.

## Permissions

**Permission**: networkmanager.serverstatus.notify\
Allows you to receive notifications when a server goes offline or online.

**Permission**: networkmanager.servers.bypassrestricted\
Allows you to bypass server restriction on all servers.

**Permission**: networkmanager.server.\<serverName>\
Allows you to bypass server restriction on the specified server.

## Settings

You can find these settings in the Web Interface under: Settings -> Plugin

"setting\_servermanager\_logingroup" - This is the group of servers where the players are sent to after they join the network. Usually if you're network is running offline/cracked mode you put the group where you have the authentication servers in.

"setting\_servermanager\_fallbackgroup" - This group is usually for the lobby servers.&#x20;

"setting\_servermanager\_force\_logingroup" - If you want to force the players to join the logingroup then you should enable this setting.

"setting\_servermanager\_kickmove" - If players get kicked from a server because it crashes or is just restarting they will be moved to an available fallback server in the fallbackgroup.\
\
\`setting\_servermanager\_status\_check\_interval\`  - Change the interval (defined in seconds) of the server status check task.

\
NOTE: The above settings expect the name of a servergroup as value.

## Allowed Versions options

* 1.19.4
* 1.19.3
* 1.19.1
* 1.19
* 1.18.2
* 1.18
* 1.17.1
* 1.17
* 1.16.4
* 1.16.3
* 1.16.2
* 1.16.1
* 1.16
* 1.15.2
* 1.15.1
* 1.15
* 1.14.4
* 1.14.3
* 1.14.2
* 1.14.1
* 1.14
* 1.13.2
* 1.13.1
* 1.13
* 1.12.2
* 1.12.1
* 1.12
* 1.11.2
* 1.11.1
* 1.11.x
* 1.11
* 1.10.x
* 1.10.2
* 1.10.1
* 1.10
* 1.9.3
* 1.9.4
* 1.9.3 - 1.9.4
* 1.9.2
* 1.9.1
* 1.9
* 1.8.x
* 1.8
* 1.7.6
* 1.7.7
* 1.7.8
* 1.7.9
* 1.7.10
* 1.7.6 - 1.7.10
* 1.7.2
* 1.7.3
* 1.7.4
* 1.7.5
* 1.7.2 - 1.7.5
