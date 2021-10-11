# TicketSystem

**NOTE: **The TicketSystem isn't an addon of the Web Interface!

{% hint style="warning" %}
Apache mod_security can cause issues with the ticket system!
{% endhint %}

## Features

* Authentication with the player's name as username.
* View your own tickets.
* Create tickets.
* Respond to your own tickets.
* Texteditor that allows formatting and media.
* Per-user settings. They can change language and theme.

## How to install it?

You can say the the installation instructions are pretty similar to the installation of the Web Interface and that's true. The same installation files were used but modified.

1. You'll need to download the latest version of the TicketSystem. Once downloaded unzip the file and upload the content of the ZIP into your web directory. (example: /var/www/html/networkmanager/tickets).
2. Ensure you have set 'protected/config.php' and 'inc/php/language' (folder) to permissions 777.
3. Now configure the WebInterface. Navigate to something like: 'http://YOUR_IP_OR_DOMAIN/your_path/install.php'.
4. Follow the instructions on the screen. You need your MySQL details (Same as the plugin) and ensure you have set 'protected/config.php' to permissions 777 before clicking Install Now! (Its recommended to set this back to 644 once you are done). Then you will be redirected to the login.
5. Delete the install.php and install_data.php. Thats all!

## How to change register text

By default you see this text when clicking on the "Register Now" button. If you would like to change this text then you open the login.php file in your favourite text editor and you'll see between line 250 and 263 the code of the model. Between these lines is also the text that's being shown. You're free to modify the text!

![](<../../.gitbook/assets/image (7).png>)
