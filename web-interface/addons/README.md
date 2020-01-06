# Addons

### Requirements

1. Your Web Interface needs to be installed and configured.
2. The required plugin needs to be connected to a MySQL database \(Not the NetworkManager database\)

### Installation

1. You'll need to download the latest version of Addon. Once downloaded unzip the file and upload the content of the ZIP into your web directory. \(example: /var/www/html/addons\).
2. Now configure the Addon. Navigate to something like: '[http://YOUR\_IP\_OR\_DOMAIN/YOUR\_PATH/addons/ADDON\_NAME/install.php](http://YOUR_IP_OR_DOMAIN/YOUR_PATH/addons/ADDON_NAME/install.php)'.
3. Follow the instructions on the screen. You need your MySQL details \(Same as the plugin that is required for the Addon\) and ensure you have set 'addons/ADDON\_NAME/dep/config.php' to permissions 777 before clicking Install Now! \(Its recommended to set this back to 644 once you are done\).
4. Delete the install.php and install\_data.php. Thats all!

### Common Issues

1. Cannot Write File: It means it can't write to the config.php file. You need to give it the correct permissions. Repeat step 3.
2. Cannot connect to database: Make sure the MySQL details you filled in are correct.

