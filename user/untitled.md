---
description: Get and set the user and connection settings
---

# ⚙ User settings

In order to get the right tasks, most of the connections need a configuration. This endpoint allows you to read and also set the required settings.

{% swagger method="get" path="/user/settings" baseUrl="https://api.dœcentral.com" summary="User settings" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="query" name="prettyprint" type="boolean" %}

{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

### Options of settings

The available options are available as an object in the [connections endpoint](../public/connections.md). For every connection you'll find an object called `settings`.

**Example:**

```json
    {
      "color": "#333",
      "slug": "google-calendar",
      "icon": "https://icongr.am/simple/googlecalendar.svg?size=32&colored=true",
      "name": "Google Calendar",
      "settings": {
        "calendar": {
          "type": "array",
          "desc": "List of calendar",
          "name": "Calendar"
        }
      },
      "public": true,
      "status": "Live",
      "_id": 2
    }
```
