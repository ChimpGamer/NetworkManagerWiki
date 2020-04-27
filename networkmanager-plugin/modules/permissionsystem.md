# PermissionSystem

The `[default]` user is like a template for all new users. So when a new user joins everything applied to \[default\] will apply on the new user.

### Commands

`/nmperms user <user>`  
 `/nmperms user <user> promote <ladder>`  
 `/nmperms user <user> demote <ladder>`  
 `/nmperms user <user> setrank <group>`  
 `/nmperms user <user> addgroup <group> (server) (expires)`  
 `/nmperms user <user> removegroup <group> (server) (expires)`  
 `/nmperms user <user> add <permission> (server) (world) (expires)`  
 `/nmperms user <user> remove <permission> (server) (world) (expires)`  
 `/nmperms user <user> clearperms`  
 `/nmperms user <user> delete`  
 `/nmperms user <user> create`  
 `/nmperms user <user> prefix set/remove <prefix>`  
 `/nmperms user <user> suffix set/remove <suffix>`  
 `/nmperms user <user> haspermission <permission> (server) (world)`  
 `/nmperms groups`  
 `/nmperms group <group>`  
 `/nmperms group <group> create (ladder) (rank)`  
 `/nmperms group <group> delete`  
 `/nmperms group <group> clearperms`  
 `/nmperms group <group> add <permission> (server) (world) (expires)`  
 `/nmperms group <group> remove <permission> (server) (world) (expires)`  
 `/nmperms group <group> parents add/remove <parent>`  
 `/nmperms group <group> prefix set <prefix> (server) | ... prefix remove (server)`  
 `/nmperms group <group> suffix set <suffix> (server) | ... suffix remove (server)`  
 `/nmperms group <group> setladder <ladder>`  
 `/nmperms group <group> setrank <rank>`  
 `/nmperms group <group> rename <name>`  
 `/nmperms group <group> haspermission <permission> (server) (world)`  
 `/nmperms group <group> members`  
 `/nmperms ladders`  
 `/nmperms haspermission <permission>`  
 `/nmperms reload | /nmperms globalreload`  


All server and world parameters can be replaced by "all" to indicate a global setting.  
 When removing permissions or player groups, all server, world and expiry date parameters can be replaced by "any" to remove any occurrences of that parameter.  
 Parameters within \(\)'s are optional parameters.  
 Parameters within &lt;&gt;'s are required.

### Timed permissions and groups

**Syntaxes:**  
`/nmp user add (server) (world) (expires  
/nmp group add (server) (world) (expires)  
/nmp user addgroup (server) (expires)`

Where \(expires\) is either a specific datetime with format "yyyy-MM-dd HH:mm:ss" \(24 hour clock\) or a duration, like "1m10w5min" which specifies 1 month + 10 weeks + 5 minutes. These timed features will have second accuracy.

### **Sequences**

Sequences allow you to add multiple permissions from the same plugin using one command only.  
Example:  
/nmp user &lt;user&gt; add essentials.{pay,balance,tpa,home,warp} \(Without spaces\)  
Will add the 5 permissions to the player. \(essentials.pay, essentials.balance, essentials.tpa, essentials.home, essentials.warp\)

### How to

* How do I add a default group: You can use the command `/nmperms user [default] addgroup <group>`
* How do I remove a default group: You can use the command `/nmperms user [default] removegroup <group>`
* How can I create a prefix/suffix with spaces: You can put the prefix/suffix between quotes like "&7\[ &c&lNetwork Manager &7\]"
* How can I use nmperms in my spigot console: Simple you use `/nmpb`. nmpb stands for NetworkManagerPermsBridge \(This requires you to install and configure NetworkManager on your Spigot servers\)

