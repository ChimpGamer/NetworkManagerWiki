# Player

{% swagger baseUrl="http://yourdomain.com:4777" path="/player/:uuid" method="get" summary="Get Player by UUID" %}
{% swagger-description %}
Retrieves data of the player by UUID.
{% endswagger-description %}

{% swagger-parameter in="path" name="uuid" type="string" %}
uuid of the player.
{% endswagger-parameter %}

{% swagger-parameter in="header" name="Authentication" type="string" %}
Authentication token for Basic authentication.
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
{
    "name": "John",
    "uuid": "acb4cbcb-0824-4e60-b578-0fe604008bb0",
    "server": "Survival",
    "version": "1.16.2",
    "nickname": "Peter",
    "language": "English",
    "playtime": 2632371610,
    "firslogin": 1550923060710,
    "lastlogin": 1597251171109,
    "lastlogout": 1597254899037,
    "groups": []
}
```
{% endswagger-response %}

{% swagger-response status="404" description="Could not find a player matching this query." %}
```
{"message": "Could not find player by uuid: acb4cbcb-0824-4e60-b578-0fe604008bb0"}
```
{% endswagger-response %}
{% endswagger %}

