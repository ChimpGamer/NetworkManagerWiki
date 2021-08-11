# DiscordBot

{% api-method method="get" host="http://yourdomain.com:4777" path="/discordbot/playeruuid/:id" %}
{% api-method-summary %}
Get Player UUID by Discord User Id
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=true %}
id of the discord user you want to retrieve the uuid from
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
Authentication token for basic authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
UUID successfully found
{% endapi-method-response-example-description %}

```
{"uuid": "bfae0d10-b2de-44d8-b6c9-e70387cc3aea"}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find uuid matching the given discord user id
{% endapi-method-response-example-description %}

```
{"message": "Could not find uuid by discord user id: 183723789308264457"}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="http://yourdomain.com:4777" path="/discordbot/userid/:uuid" %}
{% api-method-summary %}
Get Discord User Id by Player UUID
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="uuid" type="string" required=true %}
uuid of the player you want to retrieve the discord user id from
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Discord user id successfully found
{% endapi-method-response-example-description %}

```
{"userid": "183723789308264457"}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find discord user id matching the given player uuid
{% endapi-method-response-example-description %}

```
{"message": "Could not find discord user id by uuid: bfae0d10-b2de-44d8-b6c9-e70387cc3aea"}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

