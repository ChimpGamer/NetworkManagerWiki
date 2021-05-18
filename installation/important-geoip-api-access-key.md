# \(Important\) GeoIP Api Access Key

NetworkManager uses a third party service to get the country code of a player. This service is free to use \(with limitations\) but requires an API Key. You can get yourself a free key here: [https://ipapi.com/product](https://ipapi.com/product). 

Once you got a key go to **Web Interface** -&gt; **Settings** -&gt; **Plugin**. Here you search for the setting \`setting\_geoip\_api\_accesskey\`. Enter the new key in the field. Execute nm reload in the bungee console to apply the changes right away. If you don't see the warning anymore then it has been applied successfully.

