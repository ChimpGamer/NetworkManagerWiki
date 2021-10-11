# OnlinePlayers

{% swagger baseUrl="http://yourdomain.com:4777" path="/onlinePlayers" method="get" summary="Get OnlinePlayers" %}
{% swagger-description %}
This endpoint allows you to get free cakes.
{% endswagger-description %}

{% swagger-parameter in="header" name="Authentication" type="string" %}
Authentication token for basic authentication.
{% endswagger-parameter %}

{% swagger-response status="200" description="Cake successfully retrieved." %}
```
{
    "lobby": [],
    "survival": ["Peter", "Karel"]
}
```
{% endswagger-response %}
{% endswagger %}
