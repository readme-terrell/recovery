---
title: AT-PAYREF-IRC (Autoridade Tributária Referencia de Pagamento IRC)
excerpt: Retrieve pay references for IRC
api:
  file: bizapis.json
  operationId: at-payref-irc-autoridade-tributária-referencia-de-pagamento-irc
hidden: false
---
> ⚠️ Important Notice
>
> The "file" field may only be included in the response if the client holds a subscription that includes access to the associated file.\
> If you wish to enable this feature in your plan, please contact our sales team for further details and subscription options.

# JSON Schema for API Response

```json ENG
{
  "$schema": "https://json-schema.org/draft/2020-12/schema",
  "title": "AtPayrefIrcResponse",
  "type": "object",
  "properties": {
    "RequestId": {
      "type": "string",
      "description": "Unique identifier for the request."
    },
    "TaxSelfAssessmentList": {
      "type": "array",
      "description": "List of tax self assessments.",
      "items": {
        "type": "object",
        "properties": {
          "declarationId": {
            "type": "string",
            "description": "Declaration Identification"
          },
          "periodYear": {
            "type": "string",
            "description": "Year of the Period"
          },
          "documentId": {
            "type": "string",
            "description": "Document Identification"
          },
          "fiscalId": {
            "type": "string",
            "description": "Fiscal Identification"
          },
          "amountToPay": {
            "type": "number",
            "description": "Amount to Pay"
          },
          "paymentReference": {
            "type": "string",
            "description": "Payment Reference"
          },
          "paymentCertification": {
            "type": "string",
            "description": "Payment Certification"
          }
        },
        "required": []
      }
    }
  },
  "required": []
}

```
```json PT
{
  "$schema": "https://json-schema.org/draft/2020-12/schema",
  "title": "AtPayrefIrcResponse",
  "type": "object",
  "properties": {
    "RequestId": {
      "type": "string",
      "description": "Identificador único do pedido."
    },
    "TaxSelfAssessmentList": {
      "type": "array",
      "description": "Lista de declarações de autoavaliação fiscal.",
      "items": {
        "type": "object",
        "properties": {
          "declarationId": {
            "type": "string",
            "description": "Identificação da declaração"
          },
          "periodYear": {
            "type": "string",
            "description": "Ano do período fiscal"
          },
          "documentId": {
            "type": "string",
            "description": "Identificação do documento"
          },
          "fiscalId": {
            "type": "string",
            "description": "Número de identificação fiscal do contribuinte"
          },
          "amountToPay": {
            "type": "number",
            "description": "Montante a pagar"
          },
          "paymentReference": {
            "type": "string",
            "description": "Referência para pagamento"
          },
          "paymentCertification": {
            "type": "string",
            "description": "Código de certificação do pagamento"
          }
        },
        "required": []
      }
    }
  },
  "required": []
}

```