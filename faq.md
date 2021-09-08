---
description: A place to find all the Frequently Asked Questions Regarding NetworkManager.
---

# FAQ

## Commonly Asked Questions:

Q: Maintenance Bypass Permission Node?

A: networkmanager.maintenance.bypass

## An error occurred while fetching your user data!

\(This error could be can occur on BungeeCord & Spigot\)

This error could be caused by:

* You'll have to set bungeecord to true in the spigot.yml of the server you're connecting to.
* Another kick cause like: - "ChimpGamer disconnected with: You are already connected to this proxy!". \(To confirm this you can check your BungeeCord & spigot console\).
* If the user is new and it took too long for MySQL to handle the load it could be that when you login for the first time you'll get this error. Check the latency between your MySQL server and BungeeCord/Spigot server\(s\).

## How do I update the Web Interface?

You can use this update script \([link](https://github.com/ChimpGamer/NetworkManager/blob/master/Webbie/InstallScripts/nmpanel_update.sh)\) written by [Daniel Markink](https://github.com/DanielMarkink).

  
You can also download the zip manually, back-up the config.ini \(located at protected/config.ini\) and the settings.json \(located at protected/settings.json\), then remove all files and put the new once in. Then restore the files you've backed-up and then the update is complete.  
Another option is to remove all files, upload the new files, run the install.php and skip the create user part. Make sure to follow the WebInterface installation steps [here](https://networkmanager.gitbook.io/wiki/installation/networkmanager-webinterface).

## How do I create an announcement in multiple languages?

To achieve this you'll have to use the language system in NetworkManager. If you have multiple languages you have to create a language key for example: announcement\_discord and add this key to every language in the language messages table of NetworkManager. You can use this sql query to do this:

```sql
INSERT INTO nm_language_messages(`language_id`, `key`, `message`, `plugin`, `version`) SELECT `id`, `announcement_discord`, `Please join our discord https://discord.gg/12345`, `NetworkManager`, `1.0.0` FROM nm_languages;
```

You can fill what ever you want as version but that is mainly used to maintain the language messages used in NetworkManager. After this you can change the message in the web interface for every language.

When you've added this language key you go to the BungeeCord console and execute "nm reload languages". After you've done that you can create an announcement and simply set as message: `%message_announcement_discord%`

