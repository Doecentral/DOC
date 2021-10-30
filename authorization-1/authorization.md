---
cover: >-
  https://images.unsplash.com/photo-1609770231080-e321deccc34c?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHwyfHxLZXl8ZW58MHx8fHwxNjM0Njc2MjMz&ixlib=rb-1.2.1&q=85
coverY: 0
---

# 🔐 Authorization

The dœcentral API is using API keys as authorization.&#x20;

```http
# Basic request with authorization
GET /tasks/today?prettyprint=true
Authorization: Bearer <YOUR_API_KEY>
Accept: application/json
```

The API keys can be managed at [https://app.dœcentral.com/?settings\&apikeys](https://app.xn--dcentral-ktb.com/?settings\&apikeys)
