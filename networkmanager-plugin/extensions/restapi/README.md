---
description: Only applies to RestAPI v2.0.0 and newer
---

# RestAPI

This still has to be completed but it's enough for basic usage.

## How to use?

1. Enable the RestAPI in the settings.yml of the RestAPI extension \(NetworkManager BungeeCord\).
2. Make sure the port you are using is open \(free\) and not blocked by the firewall.
3. Copy the secret. Open the WebInterface and go to settings. Paste the secret in the "secret" text field.
4. Enter the a valid api url. Like [http://yourbungeecordserver.com:4777](http://google.nl:777/) or if you use https://[yourbungeecordserver.com](http://google.nl:777/)[:8777](https://google.nl:8777/).
5. Now you need an addon that works with the RestAPI. You can find some in the Discord.

If there is something wrong. Always check the console log of the browser. And remember! Your browser cache can be a B!tch.

NOTE: It is recommended to use HTTPS. HTTPS will only be activated if there is a valid keystore file in the keystore-path. HTTP will be disabled if you use HTTPS.

~~If the RestAPI doesn't work it is probably because you use BungeeCord. For some odd reason the RestAPI doesn't work with BungeeCord but it does with Waterfall. I'm not sure about other forks of BungeeCord.~~

