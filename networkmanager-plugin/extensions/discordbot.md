# DiscordBot

## Features

* Verification system to connect Discord accounts with MC accounts.
* Username and Rank sync. \(Rank sync works with NMPerms, PowerfulPerms, LuckPerms and UltraPermissions\)
* Connect the staffchat and adminchat from networkmanager with discord. You can even interact with them trough discord.
* You can change the status of your discord bot.
* Configurable command prefix.
* Receive notification from several events like HelpOP requests, Punishments or Server status changes.
* Make the bot send messages from all mc servers or just one to a specific discord channel.

## How to install?

1. [Download ](https://discord.com/channels/222070253172031500/564936239413985321)the extension from the Discord server.
2. Drop the extension jar in the extensions folder on your BungeeCord server.
3. Restart your BungeeCord server.
4. Configure the DiscordBot Extension by opening the settings.yml of the DiscordBot extension with a text editor. \(The most important things are the token and the guildId\)
5. Restart your BungeeCord server and if you configured it right you should see the discord bot online in your discord server.

NOTE: Make sure you check this: [https://github.com/DV8FromTheWorld/JDA/wiki/19%29-Troubleshooting\#im-getting-closecode4014--disallowed-intents](https://github.com/DV8FromTheWorld/JDA/wiki/19%29-Troubleshooting#im-getting-closecode4014--disallowed-intents) and enable "SERVER MEMBERS INTENT"!

Check: [https://github.com/DV8FromTheWorld/JDA/wiki/19%29-Troubleshooting](https://github.com/DV8FromTheWorld/JDA/wiki/19%29-Troubleshooting)

## How do I link my discord account?

1. PM the discord bot "!register".
2. The bot will send you a key you have to copy.
3. Then you execute /register &lt;key&gt; in-game and you will be verified. \(Permission: networkmanager.bot.register\)
4. The key message got edited by the bot telling you the verification process has succeeded.

## Commands

!register - PM to Bot Only  
!players/!online/!onlineplayers  
!playtime  
!uptime

In-game:  
- /bug - networkmanager.bot.bug  
- /suggestion - networkmanager.bot.suggestion  
- /register - networkmanager.bot.register  
- /unregister - networkmanager.bot.unregister  
- /discord - no permission  
- /nmbot - networkmanager.admin

NOTE: Some commands can be changed in the configuration

## Placeholders

DiscordBot adds a couple of placeholders to NetworkManager. You can use those placeholders in announcements or other messages.

| Placeholder | Description |
| :--- | :--- |
| %discordbot\_guild\_id% | Returns the ID of the Discord guild |
| %discordbot\_guild\_name% | Returns the name of the Discord guild |
| %discordbot\_members\_online% | Returns the amount of online members |
| %discordbot\_members\_total% | Returns the amount of total members |

