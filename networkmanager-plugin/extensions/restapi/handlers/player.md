# Player

{% api-method method="get" host="http://yourdomain.com:4777" path="/player/:uuid" %}
{% api-method-summary %}
Get Player by UUID
{% endapi-method-summary %}

{% api-method-description %}
Retrieves data of the player by UUID.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="uuid" type="string" required=true %}
uuid of the player.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
Authentication token for Basic authentication.
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "name": "John",
    "uuid": "acb4cbcb-0824-4e60-b578-0fe604008bb0",
    "server": "Survival",
    "version": "1.16.2",
    "language": "English",
    "playtime": 2632371610,
    "firslogin": 1550923060710,
    "lastlogin": 1597251171109,
    "lastlogout": 1597254899037,
    "groups": []
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a player matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "Could not find player by uuid: bfae0d10-b2de-44d8-b6c9-e70387cc3ae"}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



