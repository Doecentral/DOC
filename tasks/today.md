---
description: Get all the tasks for today
---

# ✅ Today

{% swagger baseUrl="https://api.dœcentral.com" path="/tasks/today" method="get" summary="Today" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="header" name="Authentication" type="string" required="true" %}
Authentication token to track down who is emptying our stocks.
{% endswagger-parameter %}

{% swagger-parameter in="query" name="overdue" type="boolean" %}
The API will do its best to find a cake matching the provided recipe.
{% endswagger-parameter %}

{% swagger-parameter in="query" name="prettyprint" type="boolean" %}
Whether the cake should be gluten-free or not.
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="Tasks successfully retrieved." %}
```
{    "name": "Cake's name",    "recipe": "Cake's recipe name",    "cake": "Binary cake"}
```
{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="Could not find a cake matching this query." %}
```
{
    "status": "error",
    "message": "Please check your API key."
}
```
{% endswagger-response %}
{% endswagger %}

