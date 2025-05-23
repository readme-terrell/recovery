---
title: Retrieve persistent data
excerpt: >-
  Endpoint to retrieve persistent data using the property requestId of bizAPIs,
  in case a service takes too long (more than 30 seconds) to give a response.
api:
  file: bizapis.json
  operationId: retrieve-persistent-data
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
# Download Project

- [Java](https://we.tl/t-fMY1oPTzwX)
- [Python](https://we.tl/t-3cU0hEbMDr)
- [C#](https://we.tl/t-9kd4abucY3)

[Watch the video](https://www.bizapis.com/wp-content/uploads/2024/08/retrieve-persistent-data.mp4.mp4)

# JSON Schema API Response

## Portuguese (PT)

```json
{
  "type": "object",
  "properties": {
    "data": {
      "type": "object",
      "properties": {
        "requestId": {
          "type": "string",
          "description": "Identificador único do pedido"
        }
      }
    },
    "file": {
      "type": "string",
      "description": "Ficheiro PDF em base 64"
    }
  }
}
```

## English (ENG)

```json
{
  "type": "object",
  "properties": {
    "data": {
      "type": "object",
      "properties": {
        "requestId": {
          "type": "string",
          "description": "Unique request identifier"
        }
      }
    },
    "file": {
      "type": "string",
      "description": "Encoded base 64 file."
    }
  }
}