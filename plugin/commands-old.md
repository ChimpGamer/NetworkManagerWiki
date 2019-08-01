# Commands \(Old\)

## NetworkManager

NOTE: Some commands require a specific module to be Enabled!

| Command | Permission | Description |
| :--- | :--- | :--- |
| `/networkmanager` | `networkmanager.admin` | Shows the help page of the main commands |
| `/networkmanager reload` | `networkmanager.admin` | Reloads the cache and uploads data to the database |
| `/networkmanager test` | `networkmanager.admin` | Shows the help page of all test commands |
| `/nmperms` | `networkmanager.permissions` | Shows all commands regarding the permissions |

### Punishments

| Command | Permission | Description |
| :--- | :--- | :--- |
| `/gban <username> <reason>` | `networkmanager.punishment.gban` | Global Ban Command |
| `/gtempban <username> <duration> <reason> (duration could be 7d for 7 days. 1mo for 1 month etc)` | `networkmanager.punishment.gtempban` | Global Temp Ban Command |
| `/gipban <username> <reason>` | `networkmanager.punishment.gipban` | Global IP Ban Command |
| `/gtempipban <username> <duration> <reason> (duration could be 7d for 7 days. 1mo for 1 month etc)` | `networkmanager.punishment.gtempipban` | Global IP Temp Ban Command |
| `/gmute <username> <reason>` | `networkmanager.punishment.gmute` | Global Mute Command |
| `/gtempmute <username> <duration> <reason> (duration could be 7d for 7 days. 1mo for 1 month etc)` | `networkmanager.punishment.gtempmute` | Global Temp Mute Command |
| `/gipmute <username> <reason>` | `networkmanager.punishment.gipmute` | Global IP Mute Command |
| `/gtempipmute <username> <duration> <reason> (duration could be 7d for 7 days. 1mo for 1 month etc)` | `networkmanager.punishment.gtempipmute` | Global Temp IP Mute Command |
| `/gkick <username> <reason>` | `networkmanager.punishment.gkick` | Global Kick Command |
| `/ban <username> <server> <reason>` | `networkmanager.punishment.ban` | Ban Command |
| `/tempban <username> <server> <duration> <reason> (duration could be 7d for 7 days. 1mo for 1 month etc)` | `networkmanager.punishment.tempban` | Temp Ban Command |
| `/ipban <username> <server> <reason>` | `networkmanager.punishment.ipban` | IP Ban Command |
| `/mute <username> <server> <reason>` | `networkmanager.punishment.mute` | Mute Command |
| `/tempmute <username> <server> <duration> <reason> (duration could be 7d for 7 days. 1mo for 1 month etc)` | `networkmanager.punishment.tempmute` | Temp Mute Command |
| `/ipmute <username> <server> <reason>` | `networkmanager.punishment.ipmute` | IP Mute Command |
| `/kick <username> <server> <reason>` | `networkmanager.punishment.kick` | Kick Command |
| `/warn <username> <reason>` | `networkmanager.punishment.warn` | Warn Command |
| `/report <username> <reason>` | `networkmanager.punishment.report` | Report Command |
| `/note <username> <reason>` | `networkmanager.punishment.note` | Note Command |
| `/gunban <username>` | `networkmanager.punishment.gunban` | Global Unban Command |
| `/gunmute <username>` | `networkmanager.punishment.gunmute` | Global Unmute Command |
| `/unban <username> <server>` | `networkmanager.punishment.unban` | Unban Command |
| `/unmute <username> <server>` | `networkmanager.punishment.unmute` | Unmute Command |

### Permissions

| Command | Permission | Description |
| :--- | :--- | :--- |
| `/nmperms user [username] add [permission]` | `networkmanager.permissions.user.add` | User permission add Command |
| `/nmperms user [username] remove[permission]` | `networkmanager.permissions.user.remove` | User permission remove Command |
| `/nmperms user [username] clearperms` | `networkmanager.permissions.user.clearperms` | User clearperms Command |
| `/nmperms user [username] addgroup [group] (server) (expires)` | `networkmanager.permissions.user.addgroup` | User add group Command |
| `/nmperms user [username] removegroup [group] (server)` | `networkmanager.permissions.user.removegroup` | User remove group Command |
| `/nmperms user [username] setrank [group]` | `networkmanager.permissions.user.setrank` | User set rank Command |
| `/nmperms user [username] promote [ladder]` | `networkmanager.permissions.user.promote` | User promote Command |
| `/nmperms user [username] demote [ladder]` | `networkmanager.permissions.user.demote` | User demote Command |
| `/nmperms user [username] prefix set [prefix]` | `networkmanager.permissions.user.prefix` | User set prefix Command |
| `/nmperms user [username] suffix set [suffix]` | `networkmanager.permissions.user.suffix` | User set suffix Command |
| `/nmperms user [username] prefix remove` | `networkmanager.permissions.user.prefix` | User remove prefixCommand |
| `/nmperms user [username] suffix remove` | `networkmanager.permissions.user.suffix` | User remove suffix Command |
| `/nmperms user [username] haspermission [permission]` | `networkmanager.permissions.user.haspermission` | User has permission Command |
| `/nmperms user [username]` | `networkmanager.permissions.user` | User info Command |
| `/nmperms group [group] create [ladder] [rank]` | `networkmanager.permissions.group.create` | Group create Command |
| `/nmperms group [group] delete` | `networkmanager.permissions.group.delete` | Group delete Command |
| `/nmperms group [group] rename [name]` | `networkmanager.permissions.group.rename` | Group rename Command |
| `/nmperms group [group] setladder [ladder]` | `networkmanager.permissions.group.setladder` | Group setladder Command |
| `/nmperms group [group] setrank [rank]` | `networkmanager.permissions.group.setrank` | Group setrank Command |
| `/nmperms group [group] rename [name]` | `networkmanager.permissions.group.rename` | Group rename Command |
| `/nmperms group [group] add [permission] (server) (world) (expires)` | `networkmanager.permissions.group.add` | Group add permission Command |
| `/nmperms group [group] remove [permission] (server) (world) (expires)` | `networkmanager.permissions.group.remove` | Group remove permission Command |
| `/nmperms group [group] parents` | `networkmanager.permissions.group.parents` | Group parent Command |
| `/nmperms group [group] parents remove [parent]` | `networkmanager.permissions.group.parents` | Group remove parent Command |
| `/nmperms group [group] parents add [parent]` | `networkmanager.permissions.group.parents` | Group add parent Command |
| `/nmperms group [group] parents remove [parent]` | `networkmanager.permissions.group.parents` | Group remove parent Command |
| `/nmperms group [group] clearperms` | `networkmanager.permissions.group.clearperms` | Group clearperms Command |
| `/nmperms group [group] prefix set [prefix]` | `networkmanager.permissions.group.prefix` | Group prefix Command |
| `/nmperms group [group] suffix set [suffix]` | `networkmanager.permissions.group.suffix` | Group suffix Command |
| `/nmperms group [group] prefix remove` | `networkmanager.permissions.group.prefix` | Group prefix Command |
| `/nmperms group [group] suffix remove` | `networkmanager.permissions.group.suffix` | Group suffix Command |
| `/nmperms group [group] haspermission [permission]` | `networkmanager.permissions.group.haspermission` | Group haspermission Command |
| `/nmperms group [group] members` | `networkmanager.permissions.group.members` | Group members Command |
| `/nmperms group [group]` | `networkmanager.permissions.group` | Group info Command |
| `/nmperms groups` | `networkmanager.permissions.groups` | Groups Command |
| `/nmperms ladders` | `networkmanager.permissions.ladders` | ladders Command |
| `/nmperms reload (global)` | `networkmanager.permissions.reload` | reload Command |

### Party

| Command | Permission | Description |
| :--- | :--- | :--- |
| `/party chat (toggle/message)` | `networkmanager.party.chat` | Party chat command |
| `/party invite <user>` | `networkmanager.party.invite` | Party invitecommand |
| `/party join <user>` | `networkmanager.party.join` | Party join command |
| `/party jump` | `networkmanager.party.jump` | Party jump command |
| `/party kick <user>` | `networkmanager.party.kick` | Party kick command |
| `/party leave` | `networkmanager.party.leave` | Party leave command |
| `/party setowner <user>` | `networkmanager.party.setowner` | Party setowner command |
| `/party setpublic <true/false>` | `networkmanager.party.setpublic` | Party setpublic command |
| `/party status` | `networkmanager.party.status` | Party statuscommand |

### Chat

| Command | Permission | Description |
| :--- | :--- | :--- |
| `/staffchat <message>` | `networkmanager.staffchat` | Staffchat command |
| `/staffchat toggle` | `networkmanager.staffchat` | Staffchat toggle command |
| `/adminchat <message>` | `networkmanager.adminchat` | Adminchat command |
| `/adminchat toggle` | `networkmanager.adminchat` | Adminchat toggle command |
| `/chatlock [servername]` | `networkmanager.chatlock` | Chatlock command |
| `/clearchat <global/servername>` | `networkmanager.clearchat` | Clearchat command |
| `/chatlog <username>` | `networkmanager.chatlog` | Chalog command |
| `/msg <username> <message>` | `networkmanager.msg` | Msg command |
| `/msg toggle` | `networkmanager.msg` | Msg toggle command |
| `/reply <message>` | `networkmanager.msg` | Reply command |
| `/helpop <message>` | `networkmanager.helpop` | Helpop command |
| `/announce <global/servername> <message>` | `networkmanager.announce` | Announce command |
| `/socialspy` | `networkmanager.socialspy` | Socialspy command |

### Others

| Command | Permission | Description |
| :--- | :--- | :--- |
| `/ping (username)` | `networkmanager.ping/networkmanager.ping.other` | Ping command |
| `/playtime (username/top)` | `networkmanager.playtime/networkmanager.playtime.other/networkmanager.playtime.top` | Playtime command |
| `/find <username>` | `networkmanager.find` | Find command |
| `/gtps` | `networkmanager.gtps` | Gtps command |
| `/lookup <username>` | `networkmanager.lookup` | Lookup command |
| `/maintenance <toggle/enable/disable/status>` | `networkmanager.maintenance/networkmanager.maintenance.toggle/networkmanager.maintenance.enable/networkmanager.maintenance.disable/networkmanager.maintenance.status/networkmanager.maintenance.*` | Maintenancemode command |
| `/nick (off/reset/username/nickname)` | `networkmanager.nickname/networkmanager.nickname.other` | Nickname command |
| `/seen <username>` | `networkmanager.seen` | Seen command |
| `/staff list` | `networkmanager.staff` | Staff command |
| `/ticket <list/register/create/respond> (password/title/ticket-id) (message)` | `networkmanager.tickets` | Ticket command |
| `/language <language>` | `networkmanager.language` | Language command |
| `/execute <allproxies/server/proxyid> <command>` | `networkmanager.execute` | Execute command |
| `/notify` | `networkmanager.notify` | notify command \(Toggles in-game notifications\) |

## Some Permissions

Colors:

* networkmanager.color.black
* networkmanager.color.dark\_blue
* networkmanager.color.dark\_green
* networkmanager.color.dark\_aqua
* networkmanager.color.dark\_red
* networkmanager.color.dark\_purple
* networkmanager.color.gold
* networkmanager.color.gray
* networkmanager.color.dark\_gray
* networkmanager.color.blue
* networkmanager.color.green
* networkmanager.color.aqua
* networkmanager.color.red
* networkmanager.color.light\_purple
* networkmanager.color.white
* networkmanager.color.rainbow

Punishments:

* networkmanager.punishment.gban.alert
* networkmanager.punishment.gtempban.alert
* networkmanager.punishment.gipban.alert
* networkmanager.punishment.gmute.alert
* networkmanager.punishment.gtempmute.alert
* networkmanager.punishment.gipmute.alert
* networkmanager.punishment.gkick.alert
* networkmanager.punishment.ban.alert
* networkmanager.punishment.tempban.alert
* networkmanager.punishment.ipban.alert
* networkmanager.punishment.mute.alert
* networkmanager.punishment.tempmute.alert
* networkmanager.punishment.ipmute.alert
* networkmanager.punishment.kick.alert
* networkmanager.punishment.warn.alert
* networkmanager.punishment.report.alert
* networkmanager.punishment.note.alert

Others:

* networkmanager.notify.joinbanned
* networkmanager.notify.\*
* networkmanager.adminchat
* networkmanager.announce
* networkmanager.announce.server
* networkmanager.announce.global
* networkmanager.announce.\*
* networkmanager.chatlock
* networkmanager.chatlog
* networkmanager.clearchat.bypass
* networkmanager.clearchat.\*
* networkmanager.find
* networkmanager.gtps
* networkmanager.helpop
* networkmanager.helpop.notify
* networkmanager.notify.ticket.new
* networkmanager.lookup
* networkmanager.lookup.ip
* networkmanager.maintenance
* networkmanager.maintenance.toggle
* networkmanager.maintenance.enable
* networkmanager.maintenance.disable
* networkmanager.maintenance.status
* networkmanager.maintenance.\*
* networkmanager.msg
* networkmanager.nickname
* networkmanager.permissions
* networkmanager.ping
* networkmanager.ping.other
* networkmanager.ping.\*
* networkmanager.playtime
* networkmanager.playtime.other
* networkmanager.playtime.top
* networkmanager.playtime.\*
* networkmanager.reports
* networkmanager.seen
* networkmanager.socialspy
* networkmanager.staffchat
* networkmanager.staff
* `networkmanager.slashserver.<servername>`
* networkmanager.slashserver.\*
* networkmanager.tickets
* networkmanager.chatlock.bypass
* networkmanager.anticaps.bypass
* networkmanager.antispam.bypass
* networkmanager.commandblocker.bypass
* networkmanager.maintenance.bypass
* networkmanager.notification.join
* networkmanager.fullproxy.bypass
* networkmanager.tabcompletechat
* networkmanager.reports.gui
* networkmanager.lookup.gui
* networkmanager.punishment.gui
* networkmanager.tags.gui
* networkmanager.tags.create
* networkmanager.tags.delete
* networkmanager.tags.setdescription
* networkmanager.tags.set
* networkmanager.tags.unset
* networkmanager.tags.
* networkmanager.tags.\*
* networkmanager.party.\*
* networkmanager.party.nolimit

