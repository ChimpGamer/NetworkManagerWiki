# TicketSystem

**NOTE:** The TicketSystem isn't an addon of the Web Interface!

{% hint style="warning" %}
Apache mod\_security can cause issues with the ticket system!
{% endhint %}

## How to install it?

You can say the the installation instructions are pretty similar to the installation of the Web Interface and that's true. The same installation files were used but modified.

1. You'll need to download the latest version of the TicketSystem. Once downloaded unzip the file and upload the content of the ZIP into your web directory. \(example: /var/www/html/networkmanager/ticketsystem\).
2. Ensure you have set 'inc/php/protected/config.php' and 'inc/php/language' \(folder\) to permissions 777.
3. Now configure the WebInterface. Navigate to something like: 'http://YOUR\_IP\_OR\_DOMAIN/your\_path/install.php'.
4. Follow the instructions on the screen. You need your MySQL details \(Same as the plugin\) and ensure you have set 'inc/php/dep/protected/config.php' to permissions 777 before clicking Install Now! \(Its recommended to set this back to 644 once you are done\). Then you will be redirected to the login.
5. Delete the install.php and install\_data.php. Thats all!

