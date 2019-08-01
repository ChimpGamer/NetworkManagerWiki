# DiscordBot

## How to use?

1. Download the extension from the Discord server.
2. Drop the extension jar in the extensions folder on your BungeeCord server.
3. Restart your BungeeCord server.
4. Configure the DiscordBot Extension by opening the settings.yml of the DiscordBot extension with a texteditor. \(The most important things are the token and the guildId\)
5. Restart your BungeeCord server and if you configured it right you should see the discord bot online in your discord server.

## Features

* Verification system to connect Discord accounts with MC accounts.
* Username and Rank sync. \(Rank sync works with NMPerms, PowerfulPerms, LuckPerms and UltraPermissions\)
* Connect the staffchat and adminchat from networkmanager with discord. You can even interact with them trough discord.
* You can change the status of your discord bot.
* Configurable command prefix.
* Receive notification from several events like HelpOP requests, Punishments or Server status changes.
* Make the bot send messages from all mc servers or just one to a specific discord channel.

## How do I link my discord account?

1. PM the discord bot "!register".
2. The bot will send you a key you have to copy.
3. Then you execute /verify &lt;key&gt; in-game and you will be verified. \(Permission: networkmanager.bot.verify\)
4. The key message got edited by the bot telling you the verification process has succeeded.

## Commands

!register - PM to Bot Only  
!unregister - PM to Bot Only  
!players/!online/!onlineplayers  
!playtime

In-game:  
- /bug - networkmanager.bot.bug  
- /suggestion - networkmanager.bot.suggestion  
- /discord - no permission  
- /nmbot - networkmanager.admin

## Extras

Did you know that when you are using the DiscordBot extension you can use the %discordbot\_users% in announcements? This allows you to make an announcement like: %discordbot\_users% already players already registered on our discord server! Will you be the next one?

