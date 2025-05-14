---
title: AT-PAYREF-IMI (Autoridade Tributária Referencia de Pagamento IMI)
excerpt: Retrieve pay references for IMI
api:
  file: bizapis.json
  operationId: at-payref-imi-autoridade-tributária-referencia-de-pagamento-imi
deprecated: false
hidden: true
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
# JSON Schema for API Response

```json PT
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "title": "AtPayrefImiResponse",
  "type": "object",
  "properties": {
    "RequestId": {
      "type": "string",
      "description": "Identificador único para a solicitação"
    },
    "Billing Note": {
      "type": "array",
      "description": "Lista de notas de cobrança.",
      "items": {
        "type": "object",
        "properties": {
          "billingNoteNumber": {
            "type": "string",
            "description": "Identificador único para a nota de cobrança"
          },
          "value": {
            "type": "number",
            "description": "Valor da nota de cobrança"
          },
          "paymentDueDate": {
            "type": "string",
            "description": "Data de vencimento da nota de cobrança"
          },
          "situation": {
            "type": "string",
            "description": "Situação ou status da nota de cobrança"
          },
          "bankReference": {
            "type": "string",
            "description": "Referência bancária associada à nota de cobrança"
          },
          "numberOfBuildings": {
            "type": "integer",
            "description": "Número de edifícios associados à nota de cobrança"
          },
          "year": {
            "type": "string",
            "description": "Ano da nota de cobrança"
          }
        },
        "required": ["billingNoteNumber", "value", "paymentDueDate", "situation", "bankReference", "numberOfBuildings", "year"]
      }
    }
  },
  "required": ["RequestId", "Billing Note"]
}

```
```json ENG
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "title": "AtPayrefImiResponse",
  "type": "object",
  "properties": {
    "RequestId": {
      "type": "string",
      "description": "Unique identifier for the request"
    },
    "Billing Note": {
      "type": "array",
      "description": "List of billing notes.",
      "items": {
        "type": "object",
        "properties": {
          "billingNoteNumber": {
            "type": "string",
            "description": "Unique identifier for the billing note"
          },
          "value": {
            "type": "number",
            "description": "Value of the billing note"
          },
          "paymentDueDate": {
            "type": "string",
            "description": "Payment due date for the billing note"
          },
          "situation": {
            "type": "string",
            "description": "Situation or status of the billing note"
          },
          "bankReference": {
            "type": "string",
            "description": "Bank reference associated with the billing note"
          },
          "numberOfBuildings": {
            "type": "integer",
            "description": "Number of buildings associated with the billing note"
          },
          "year": {
            "type": "string",
            "description": "Year of the billing note"
          }
        },
        "required": ["billingNoteNumber", "value", "paymentDueDate", "situation", "bankReference", "numberOfBuildings", "year"]
      }
    }
  },
  "required": ["RequestId", "Billing Note"]
}

```
