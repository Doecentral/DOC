---
description: Get all the tasks for tomorrow
---

# ☑ Tomorrow

{% swagger baseUrl="https://api.dœcentral.com" path="/tasks/tomorrow" method="get" summary="Tomorrow" %}
{% swagger-description %}
This endpoint allows you to get free cakes.
{% endswagger-description %}

{% swagger-parameter in="header" name="Authentication" type="string" %}

{% endswagger-parameter %}

{% swagger-parameter in="query" name="overdue" type="boolean" %}

{% endswagger-parameter %}

{% swagger-response status="200" description="Cake successfully retrieved." %}
```
{    "name": "Cake's name",    "recipe": "Cake's recipe name",    "cake": "Binary cake"}
```
{% endswagger-response %}

{% swagger-response status="404" description="Could not find a cake matching this query." %}
```
{    "message": "Ain't no cake like that."}
```
{% endswagger-response %}
{% endswagger %}

