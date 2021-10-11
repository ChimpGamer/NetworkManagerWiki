# DiscordBot

{% swagger baseUrl="http://yourdomain.com:4777" path="/discordbot/playeruuid/:id" method="get" summary="Get Player UUID by Discord User Id" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="id" type="string" %}
id of the discord user you want to retrieve the uuid from
{% endswagger-parameter %}

{% swagger-parameter in="header" name="Authentication" type="string" %}
Authentication token for basic authentication
{% endswagger-parameter %}

{% swagger-response status="200" description="UUID successfully found" %}
```
{"uuid": "bfae0d10-b2de-44d8-b6c9-e70387cc3aea"}
```
{% endswagger-response %}

{% swagger-response status="404" description="Could not find uuid matching the given discord user id" %}
```
{"message": "Could not find uuid by discord user id: 183723789308264457"}
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="http://yourdomain.com:4777" path="/discordbot/userid/:uuid" method="get" summary="Get Discord User Id by Player UUID" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="uuid" type="string" %}
uuid of the player you want to retrieve the discord user id from
{% endswagger-parameter %}

{% swagger-parameter in="header" name="Authentication" type="string" %}
Authentication token for basic authentication
{% endswagger-parameter %}

{% swagger-response status="200" description="Discord user id successfully found" %}
```
{"userid": "183723789308264457"}
```
{% endswagger-response %}

{% swagger-response status="404" description="Could not find discord user id matching the given player uuid" %}
```
{"message": "Could not find discord user id by uuid: bfae0d10-b2de-44d8-b6c9-e70387cc3aea"}
```
{% endswagger-response %}
{% endswagger %}
