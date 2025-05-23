---
title: IRSByUserPassword Details (Imposto sobre o Rendimento das Pessoas Singulares)
excerpt: Endpoint to retrieve information from the IRS Mod3 document.
api:
  file: bizapis.json
  operationId: irsbyuserpassword-imposto-sobre-o-rendimento-das-pessoas-singulares-details
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

- [Java](https://we.tl/t-joAUO6NZlJ)
- [Python](https://we.tl/t-RMtHpM3KKU)
- [C#](https://we.tl/t-0rXaS2WgvY)

[Watch the video](https://www.bizapis.com/wp-content/uploads/2024/08/servico-irs_by_user_password.mp4.mp4)

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
```