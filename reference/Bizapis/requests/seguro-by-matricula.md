---
title: Seguro-by-matricula
excerpt: >-
  This endpoint allows users to search for the insurance company of a vehicle by
  using the license plate. It also requests a date, that corresponds to the date
  to be search, allowing to search for old insurances.
api:
  file: bizapis.json
  operationId: seguro-by-matricula
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

- [Java](https://we.tl/t-81vjiKA2se)
- [Python](https://we.tl/t-tp5A6oryZi)
- [C#](https://we.tl/t-cj2IyPalDn)

[Watch the video](https://www.bizapis.com/wp-content/uploads/2024/08/servico_seguro-by-matricula.mp4.mp4)

# JSON Schema API Response

## Portuguese (PT)

```json
{
  "type": "object",
  "properties": {
    "requestId": {
      "type": "string",
      "description": "Identificador único do pedido"
    },
    "licensePlate": {
      "type": "string",
      "description": "Matrícula do veículo"
    },
    "entity": {
      "type": "string",
      "description": "Seguradora"
    },
    "startDate": {
      "type": "string",
      "description": "Data de início do seguro"
    },
    "endDate": {
      "type": "string",
      "description": "Data de fim do seguro"
    },
    "policy": {
      "type": "string",
      "description": "Número de apólice"
    }
  }
}
```

## English (ENG)

```json
{
  "type": "object",
  "properties": {
    "requestId": {
      "type": "string",
      "description": "Unique request identifier"
    },
    "licensePlate": {
      "type": "string",
      "description": "Vehicle license plate"
    },
    "entity": {
      "type": "string",
      "description": "Insurance company"
    },
    "startDate": {
      "type": "string",
      "description": "Insurance start date"
    },
    "endDate": {
      "type": "string",
      "description": "Insurance end date"
    },
    "policy": {
      "type": "string",
      "description": "Policy number"
    }
  }
}
```