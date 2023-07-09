# Permission System

## Configurations

To enable the permission system you'll have to enable the permission modules. If you only want to use the permission system on BungeeCord you enable `module_permissions_bungee`. If you only want to use the permission system on Spigot you enable `module_permissions_spigot`. If you want to use the permission system on both you simply enable both modules.

After you enabled or disabled one of these modules you'll have to restart the bungeecord or spigot server depending on the setting you changed..

## Commands

{% content-ref url="../commands/permissions.md" %}
[permissions.md](../commands/permissions.md)
{% endcontent-ref %}

## Defaults

The `[default]` user is like a template for all new users. So when a new user joins everything applied to \[default] will apply on the new user.

### Timed permissions and groups

**Syntaxes:**\
`/nmp user add (server) (world) (expires)`\
`/nmp group add (server) (world) (expires)`\
`/nmp user addgroup (server) (expires)`

Where (expires) is either a specific datetime with format "yyyy-MM-dd HH:mm:ss" (24 hour clock) or a duration, like "1m10w5min" which specifies 1 month + 10 weeks + 5 minutes. These timed features will have second accuracy.

### **Sequences**

Sequences allow you to add multiple permissions from the same plugin using one command only.\
Example:\
/nmp user \<user> add essentials.{pay,balance,tpa,home,warp} (Without spaces)\
Will add the 5 permissions to the player. (essentials.pay, essentials.balance, essentials.tpa, essentials.home, essentials.warp)

### How to

* How do I add a default group: You can use the command `/nmperms user [default] addgroup <group>`
* How do I remove a default group: You can use the command `/nmperms user [default] removegroup <group>`
* How can I create a prefix/suffix with spaces: You can put the prefix/suffix between quotes like "&7\[ \&c\&lNetwork Manager &7]"
* How can I use nmperms in my spigot console: Simple you use `/nmpb`. nmpb stands for NetworkManagerPermsBridge (This requires you to install and configure NetworkManager on your Spigot servers)
