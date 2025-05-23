---
title: IRSByCode (Imposto sobre o Rendimento das Pessoas Singulares)
excerpt: Endpoint to retrieve the IRS document.
api:
  file: bizapis.json
  operationId: irs-imposto-sobre-o-rendimento-das-pessoas-singulares
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

- [Java](https://we.tl/t-3SOLdZPM9k)
- [Python](https://we.tl/t-bGFxk8ahA5)
- [C#](https://we.tl/t-RkPgchEPv7)

[Watch the video](https://www.bizapis.com/wp-content/uploads/2024/08/irs-by-code.mp4.mp4)

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