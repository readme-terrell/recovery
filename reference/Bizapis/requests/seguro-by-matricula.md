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
> 💻 [block:html]{"html":"<h3  style=\"text-align:center;\">DOWNLOAD PROJECT</h3>\n<ul>\n  <li><a href=\"https://we.tl/t-81vjiKA2se\" target=\"_blank\">Java</li>\n  <li><a href=\"https://we.tl/t-tp5A6oryZi\">Python</li>\n  <li><a href=\"https://we.tl/t-cj2IyPalDn\">C#</li>\n</ul>"}[/block]

[block:html]
{
  "html": "<a href=\"https://www.bizapis.com/wp-content/uploads/2024/08/servico_seguro-by-matricula.mp4.mp4\" target=\"_blank\">To watch the video click here"
}
[/block]


# JSON Schema API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "requestId" : {
      "type" : "string",
      "description" : "Identificador único do pedido"
    },
    "licensePlate" : {
      "type" : "string",
      "description" : "Matrícula do veículo"
    },
    "entity" : {
      "type" : "string",
      "description" : "Seguradora"
    },
    "startDate" : {
      "type" : "string",
      "description" : "Data de início do seguro"
    },
    "endDate" : {
      "type" : "string",
      "description" : "Data de fim do seguro"
    },
    "policy" : {
      "type" : "string",
      "description" : "Número de apólice"
    }
  }
}
```
```json ENG
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