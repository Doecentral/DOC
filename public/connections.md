---
description: List of services dœcentral is connected to
---

# 🔗 Connections

{% swagger method="get" path="/public/connections" baseUrl="https://api.dœcentral.com" summary="Get all available connections" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="query" name="prettyprint" type="boolean" %}

{% endswagger-parameter %}

{% swagger-parameter in="header" name="Accept" type="string" %}

{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
  "status": "success",
  "meta": {
    "count_page": 9
  },
  "_links": {
    "self": {
      "href": "https://api.dœcentral.com/public/connections"
    },
    "first": {
      "href": "https://api.dœcentral.com/public/connections"
    },
    "pref": {
      "href": "https://api.dœcentral.com/public/connections"
    },
    "next": {
      "href": "https://api.dœcentral.com/public/connections"
    },
    "last": {
      "href": "https://api.dœcentral.com/public/connections"
    }
  },
  "errors": [],
  "data": [
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
    },
    {
      "name": "Google Tasks",
      "slug": "google-tasks",
      "color": "#333",
      "settings": {
        "taskLists": {
          "type": "array",
          "desc": "List of task-lists",
          "name": "Task lists"
        }
      },
      "public": true,
      "icon": "https://www.dœcentral.com/img/icons/google-tasks.png",
      "status": "In progress",
      "_id": 3
    },
    {
      "settings": {
        "apiKey": {
          "type": "string",
          "desc": "Your private api key from todoist. Can be found at ...",
          "name": "API key"
        },
        "filter": {
          "name": "Filter",
          "desc": "filter used for the todoist api. e.x. @tag",
          "type": "string"
        }
      },
      "public": true,
      "name": "Todoist",
      "status": "Live",
      "slug": "todoist",
      "icon": "https://icongr.am/simple/todoist.svg?size=32&colored=true",
      "color": "#da4134",
      "_id": 9
    },
    {
      "public": true,
      "slug": "trello",
      "icon": "https://icongr.am/simple/trello.svg?size=32&colored=true",
      "status": "In progress",
      "color": "#333",
      "name": "Trello",
      "_id": 10
    },
    {
      "status": "Live",
      "slug": "ical",
      "icon": "https://www.dœcentral.com/img/icons/ical.png",
      "settings": {
        "fileUrl": {
          "type": "string",
          "desc": "Address of the ical-File",
          "name": "URL of ical-File"
        }
      },
      "name": "iCal",
      "public": true,
      "color": "#333",
      "_id": 4
    }
  ]
}
```
{% endswagger-response %}
{% endswagger %}
