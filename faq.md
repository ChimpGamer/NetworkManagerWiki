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

You can use this update script \(link\) written by  [Daniel Markink](https://github.com/DanielMarkink).  
You can also download the zip manually, back-up the config.php \(located at inc/php/dep/protected/config.php\) and the settings.json \(located at inc/json/protected/settings.json\), then remove all files and put the new once in. Then restore the files you've backed-up and then the update is complete.  
Another option is to remove all files, upload the new files, run the install.php and skip the create user part. Make sure to follow the WebInterface installation steps [here](https://networkmanager.gitbook.io/wiki/installation/networkmanager-webinterface).



