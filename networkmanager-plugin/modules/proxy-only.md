# Proxy Only

### Configuration

You can find the settings in the Web Interface under: Settings -> Plugin\
You can find the messages in the Web Interface under: Languages -> (Your language) edit

1. Enable the proxy only module (module\_proxy\_only) in the settings.
2. Execute nmb reload in your lobby/lobbies console(s) and join one of the servers.
3. If you get kicked with a message like: "Please join using our BungeeCords!" then check your lobby/lobbies console(s). A message like: "| If this is a mistake please add the IP: x.x.x.x". Add that IP to the 'setting\_proxy\_only\_allowed\_ips' setting and execute 'nmb reload' in your lobby/lobbies console(s).
4. You should be able to join now. If not, make sure that you've added the right ip to the 'setting\_proxy\_only\_allowed\_ips' setting.
5. Edit the kick message. You can customize the kick message by editing 'lang\_proxy\_only\_kick' in the languages.

{% hint style="info" %}
In the setting \`setting\_proxy\_only\_allowed\_ips\` you can add multiple IP addresses by seperating them by ", ". For example: "play.yourip.net, server.yourip.net".
{% endhint %}
