# NetworkManager \(WebInterface\)

### Requirements

1. Web Server that supports PHP 7.3 or 7.4. PHP 8 is NOT supported!
2. MySQL Server with a database and a user account. \(If your MySQL Server is on a other server then your Web Server you need to allow remote connections on your MySQL Server.\) \(MariaDB 10 Recommended \(MariaDB is a fork of MySQL\)\).
3. Connected the plugin \(NetworkManager BungeeCord\) to MySQL. _This is required so that the database is populated._
4. The NetworkManager Web Interface files from the discord server.

### Installation

TIP: You can use one of the install scripts here to install the WebServer and the NetworkManager files. This does NOT install you a MySQL server! After successfully executing the script you can go to step 3 and skip all the permission steps. If you use one of these scripts make sure you execute them as sudo. Like sudo sh script.sh. You can find the scripts [here](https://github.com/ChimpGamer/NetworkManager/tree/master/Webbie/InstallScripts)

1. You'll need to download the latest version of NetworkManager \(WebInterface\) from the NetworkManager Discord server. Once downloaded unzip the file and upload the content of the ZIP into your web directory. \(example: /var/www/html/networkmanager\).
2. Ensure you have set 'protected/config.ini', 'protected/settings.json' and 'inc/php/dep/language' \(folder\) to permissions 777 including sub folders and files. \([https://www.pluralsight.com/blog/it-ops/linux-file-permissions](https://www.pluralsight.com/blog/it-ops/linux-file-permissions)\)

**If you are using Red Hat Linux or CentOS, ensure to also run the following command:**

'chcon -t httpd\_sys\_rw\_content\_t protected/config.ini', 'chcon -t httpd\_sys\_rw\_content\_t protected/settings.json' and 'chcon -t httpd\_sys\_rw\_content\_t inc/php/dep/languages/'

**As well as:**

'setsebool httpd\_can\_network\_connect 1'

'setsebool httpd\_can\_network\_connect\_db 1'

_This is to allow for SQL connections through apache._

1. Now configure the WebInterface. Navigate to something like: 'http://YOUR\_IP\_OR\_DOMAIN/your\_path/install.php'.
2. Follow the instructions on the screen. You need your MySQL details \(Same as the plugin\) and ensure you have set 'protected/config.ini' to permissions 777 before clicking Install Now! \(Its recommended to set this back to 644 once you are done\).
3. Now you create the Admin account. \(Its preferred to give accounts the same name as they have in-game. Several functions depend on it.\). Then you will be redirected to the login.
4. Delete the install.php and install\_data.php. Thats all!

NOTE: If your BungeeCord server is not in online mode make sure to change the servermode in the Settings. Login on the Web Interface, click on settings, then click plugin, then search for servermode. You can choose: ONLINE, OFFLINE or MIXED.

### Common issues

1. Cannot Write File: It means it can't write to the config.php file. You need to give it the correct permissions. Repeat step 2. If you continue to get this issue, and you are using RHEL / CentOS, ensure to run the command specific to that OS as well.
2. Cannot connect to database: Make sure the MySQL details you filled in are correct and make sure your MySQL server allows remote connections.
3. You can't login. Make sure you have installed and configured the NetworkManager plugin on BungeeCord.
4. If you cannot change your language then the languages folder does not have write permissions or you didn't install the php curl extension. The Web Interface needs to download the language file from the internet and save it in the languages folder. Give the folder languages \(inc/php/dep/languages\) permission 777 so it will be writable. This is to allow downloading the language files.
5. If you cannot change any web interface settings then the settings.json file does not have write permissions. Give the file settings.json \(protected/settings.json\) permission 777 so you can change the settings of the WebInterface through the WebInterface.
6. If a page or some pages don't load or don't work as expected you could try to clear your browser cache. If that doesn't solve the issue check if you have an adblocker and try to disable it.
7. If a page or some pages don't load or are very slow then you might wanna check your php version. If you are using php 5.x then this could be the issue. Update your PHP version to at least 7+

