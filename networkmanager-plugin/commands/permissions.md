# Permissions

### User Permissions

| Command | Permission |
| :--- | :--- |
| /nmperms user \[username\] | networkmanager.permissions.user |
| /nmperms user \[username\] add \[permission\] | networkmanager.permissions.user.add |
| /nmperms user \[username\] remove \[permission\] | networkmanager.permissions.user.remove |
| /nmperms user \[username\] clearperms | networkmanager.permissions.user.clearperms |
| /nmperms user \[username\] addgroup \[group\] \(server\) \(expires\) | networkmanager.permissions.user.addgroup |
| /nmperms user \[username\] removegroup \[group\] \(server\) | networkmanager.permissions.user.removegroup |
| /nmperms user \[username\] setrank \(group\) | networkmanager.permissions.user.setrank |
| /nmperms user \[username\] promote \[ladder\] | networkmanager.permissions.user.promote |
| /nmperms user \[username\] demote \[ladder\] | networkmanager.permissions.user.demote |
| /nmperms user \[username\] prefix set \[prefix\] \(server\) | networkmanager.permissions.user.prefix |
| /nmperms user \[username\] suffix set \[suffix\] \(server\) | networkmanager.permissions.user.suffix |
| /nmperms user \[username\] prefix remove \(server\) | networkmanager.permissions.user.prefix |
| /nmperms user \[username\] suffix remove \(server\) | networkmanager.permissions.user.suffix |
| /nmperms user \[username\] haspermission \[permission\] \(server\) \(world\) | networkmanager.permissions.user.haspermission |

### Group Permissions

| Command | Permissions |
| :--- | :--- |
| /nmperms groups | networkmanager.permissions.groups |
| /nmperms group \[group\] | networkmanager.permissions.group |
| /nmperms group \[group\] create \[ladder\] \[rank\] | networkmanager.permissions.group.create |
| /nmperms group \[group\] delete | networkmanager.permissions.group.delete |
| /nmperms group \[group\] rename \[name\] | networkmanager.permissions.group.rename |
| /nmperms group \[group\] setladder \[ladder\] | networkmanager.permissions.group.setladder |
| /nmperms group \[group\] setrank \[rank\] | networkmanager.permissions.group.setrank |
| /nmperms group \[group\] rename \[name\] | networkmanager.permissions.group.rename |
| /nmperms group \[group\] add \[permission\] \(server\) \(world\) \(expires\) | networkmanager.permissions.group.add |
| /nmperms group \[group\] remove \[permission \(server\) \(world\) | networkmanager.permissions.group.remove |
| /nmperms group \[group\] parents | networkmanager.permissions.group.parents |
| /nmperms group \[group\] parents add \[group\] | networkmanager.permissions.group.parents |
| /nmperms group \[group\] parents remove \[group\] | networkmanager.permissions.group.parents |
| /nmperms group \[group\] clearperms | networkmanager.permissions.group.clearperms |
| /nmperms group \[group\] prefix set \[prefix\] \(server\) | networkmanager.permissions.group.prefix |
| /nmperms group \[group\] suffix set \[suffix\] \(server\) | networkmanager.permissions.group.suffix |
| /nmperms group \[group\] prefix remove \(server\) | networkmanager.permissions.group.prefix |
| /nmperms group \[group\] suffix remove \(server\) | networkmanager.permissions.group.suffix |
| /nmperms group \[group\] haspermission \[permission\] | networkmanager.permissions.group.haspermission |
| /nmperms group \[group\] members | networkmanager.permissions.group.members |
| /nmperms ladders | networkmanager.permissions.ladders |
| /nmperms reload \(global\) | networkmanager.permissions.reload |

All server and world parameters can be replaced by "all" to indicate a global setting.  
When removing permissions or player groups, all server, world and expiry date parameters can be replaced by "any" to remove any occurrences of that parameter.  
 Parameters within \(\)'s are optional parameters.  
 Parameters within \[\]'s are required.

