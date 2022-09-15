---
description: This page is a Work In Progress since 15-9
---

# BanList

{% hint style="info" %}
The banlist isn't an addon of the Web Interface!
{% endhint %}

{% hint style="warning" %}
Make sure you target the public folder as document root folder in the configuration on your webserver.
{% endhint %}

{% hint style="warning" %}
This instruction is only targeted for linux installations.
{% endhint %}

## Download Files

First you have to create a folder for you to store the files.

```shell
mkdir -p /var/www/nmbanlist
cd /var/www/nmbanlist
```

Now we download the zip file and extract it in the folder. First you have to copy the download url from the banlist channel in the NetworkManager discord.

```shell
curl -o nmbanlist.zip <url>
unzip nmbanlist.zip
```

## Installation

Create a new configuration for your webserver.

{% tabs %}
{% tab title="Apache" %}
First you have to create a new site configuration for apache. Create a file called nmbanlist.conf and place this in /etc/apache2/sites-available.\
Paste the content below in the nmbanlist.conf

```apacheconf
<VirtualHost *:80>
  ServerName <domain>
  DocumentRoot "/var/www/nmbanlist/public"
  
  <Directory "/var/www/nmbanlist/public">
    AllowOverride all
    Require all granted
  </Directory>
</VirtualHost>
```

Once you've done that you'll have to enable the configuration you just made.

```shell
sudo ln -s /etc/apache2/sites-available/nmbanlist.conf /etc/apache2/sites-enabled/nmbanlist.conf
sudo a2enmod rewrite
sudo systemctl restart apache2
```
{% endtab %}

{% tab title="Nginx" %}


```nginx
```
{% endtab %}
{% endtabs %}

Ensure you have set 'inc/classes/config.php' to permissions 777.

```shell
chmod 777 inc/classes/config.php
```

Now you navigate in your browser to http://yourdomain.com/install.php

Follow the instructions on the screen. You need your MySQL details (Same as the plugin) and ensure you have set 'inc/classes/config.php' to permissions 777 before clicking Install Now! (Its recommended to set this back to 644 once you are done).

```shell
chmod 644 inc/classes/config.php
```

That should be it! Now you can start using it!
