---
title: Responsabilidade Crédito Details
excerpt: This endpoint returns a document about the Responsabilidade Crédito.
api:
  file: bizapis.json
  operationId: responsabilidade-crédito-details
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

- [Java](https://we.tl/t-AzI2NwT01R)
- [Python](https://we.tl/t-RBmDAZqlGs)
- [C#](https://we.tl/t-wrclKxJCCa)

[Watch the video](https://www.bizapis.com/wp-content/uploads/2024/08/servico_responsabilidade_credito.mp4.mp4)

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