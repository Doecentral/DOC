---
description: Get all the tasks for today
---

# ✅ Today

The main endpoint and initial reason for dœcentral. Get all your tasks for today from all services you use in just one single endpoint.

{% swagger baseUrl="https://api.dœcentral.com" path="/tasks/today" method="get" summary="Today" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="header" name="Authentication" type="string" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="query" name="overdue" type="boolean" %}

{% endswagger-parameter %}

{% swagger-parameter in="query" name="prettyprint" type="boolean" %}

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

