---
title: AT-PAYREF-IVA (Autoridade Tributária Referencia de Pagamento IVA)
excerpt: Retrieve pay references for IVA
api:
  file: bizapis.json
  operationId: at-payref-iva-autoridade-tributária-referencia-de-pagamento-iva
hidden: false
---
> ⚠️ Important Notice
>
> The "file" field may only be included in the response if the client holds a subscription that includes access to the associated file.\
> If you wish to enable this feature in your plan, please contact our sales team for further details and subscription options.

# JSON Schema for API Response

```json ENG
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "title": "AtPayrefIvaResponse",
  "type": "object",
  "properties": {
    "RequestId": {
      "type": "string"
    },
    "Declaration": {
      "type": "object",
      "description": "Periodic IVA declaration",
      "properties": {
        "name": {
          "type": "string",
          "description": "Name of the passive subject"
        },
        "address": {
          "type": "string",
          "description": "Address of the passive subject"
        },
        "city": {
          "type": "string",
          "description": "City of the passive subject"
        },
        "postalCode": {
          "type": "string",
          "description": "Postal Code of the passive subject"
        },
        "fiscalId": {
          "type": "string",
          "description": "Fiscal Identification"
        },
        "period": {
          "type": "string",
          "description": "Period"
        },
        "declarationId": {
          "type": "string",
          "description": "Declaration ID"
        },
        "declarationDateTime": {
          "type": "string",
          "description": "Date and Time of Declaration"
        },
        "paymentReference": {
          "type": "string",
          "description": "Payment Reference"
        },
        "opticalLine": {
          "type": "string",
          "description": "Optical Line"
        },
        "amountToPay": {
          "type": "number",
          "description": "Amount to Pay"
        }
      },
      "required": [],
      "additionalProperties": false
    }
  },
  "required": [],
  "additionalProperties": false
}

```
```json PT
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "title": "AtPayrefIvaResponse",
  "type": "object",
  "properties": {
    "RequestId": {
      "type": "string",
      "description": "Identificador único do pedido"
    },
    "Declaration": {
      "type": "object",
      "description": "Declaração periódica de IVA",
      "properties": {
        "name": {
          "type": "string",
          "description": "Nome do sujeito passivo"
        },
        "address": {
          "type": "string",
          "description": "Endereço do sujeito passivo"
        },
        "city": {
          "type": "string",
          "description": "Cidade do sujeito passivo"
        },
        "postalCode": {
          "type": "string",
          "description": "Código postal do sujeito passivo"
        },
        "fiscalId": {
          "type": "string",
          "description": "Número de identificação fiscal (NIF)"
        },
        "period": {
          "type": "string",
          "description": "Período fiscal da declaração"
        },
        "declarationId": {
          "type": "string",
          "description": "Identificador da declaração"
        },
        "declarationDateTime": {
          "type": "string",
          "description": "Data e hora da submissão da declaração"
        },
        "paymentReference": {
          "type": "string",
          "description": "Referência de pagamento"
        },
        "opticalLine": {
          "type": "string",
          "description": "Linha ótica associada ao pagamento"
        },
        "amountToPay": {
          "type": "number",
          "description": "Valor a pagar"
        }
      },
      "required": [],
      "additionalProperties": false
    }
  },
  "required": [],
  "additionalProperties": false
}

```