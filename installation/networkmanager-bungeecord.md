# NetworkManager \(BungeeCord\)

![](../.gitbook/assets/image.png)

### Requirements

1. Make sure you have Java 8 installed!​
2. BungeeCord Server that is configured.
3. MySQL Server with a database and a user account. \(If your MySQL Server is on a other server then your Web Server you need to allow remote connections on your MySQL Server.\) \(MariaDB 10 Recommended \(MariaDB is a fork of MySQL\)\).

### Installation

1. Drop the plugin \(NetworkManager\) in your BungeeCord plugins folder.
2. Start your BungeeCord server.
3. Open the settings.yml located at /plugins/NetworkManager/settings.yml.
4. Enter your MySQL host, port, username, password and database.
5. \(Optional\) Enable Redis. Enter redis host and password if you set one.
6. Restart your BungeeCord server. It will now create tables and insert some data into it.
7. Execute "nm test database" in the console to test the connection. If the command is unknown check your bungeecord log.

{% hint style="danger" %}
Don't join the server yet! After you installed the WebInterface go to the Settings and search for servermode. Make sure you've set the correct servermode.   
  
You can choose: ONLINE, OFFLINE or MIXED.
{% endhint %}

### Settings explained

The settings.yml has a couple of settings.

```yaml
networkmanager:
  mysql:
    storage: MYSQL # You can choose MYSQL OR MARIADB
    host: localhost # The IP or DNS-name of your MYSQL server.
    port: 3306 # The port of your MYSQL server.
    database: db_NetworkManager # The database you created for NetworkManager on your MYSQL server
    username: NetworkManager # The username that has access to the database
    password: NetworkManager # The password for the account on your MYSQL server.
    pool-settings: # Don't touch the pool-settings unless you know what you are doing!
      maximum-size: 10 
      minimum-idle: 10
      maximum-lifetime: 180000
      connection-timeout: 5000
    usessl: false
  redis:
    enabled: false # Enable Redis if you have a redis server.
    host: localhost # The IP or DNS-name of your redis server.
    port: 6379 # The port of your redis server.
    password: password # The password of your redis server.
  rabbitmq:
    enabled: true
    host: localhost
    port: 5672
    username: username
    password: password
  updater:
    enabled: false # Enable the spigot updater (This has to be enabled if you want to use the /nm update command)
    username: '' # Your spigot username.
    password: '' # Your spigot password
    2fasecret: '' # Your 2fa secrect (You only have to fill this in if you have 2fa enabled).
  updatechecker: true # This will check if there is an update for NetworkManager available and will notify you about it!
  debug: true # Enabled/Disable debugging. Debugging can help you to find some issues or get extra information in your server console.
```

### Common issues

1. If you see something like this: "Could not create connection to database server. Attempted reconnect 3 times. Giving up." it means it couldn't connect to your MySQL database. Check in the setting.yml if you have set the correct settings.

