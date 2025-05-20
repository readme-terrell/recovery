---
title: AT-IVA- SA (Autoridade Tributária-IVA Situação Atual)
excerpt: >-
  Endpoint to retrieve the list of IVA (Imposto sobre Valor Acrescentado
  Situação Atual) in Autoridade Tributária.
api:
  file: bizapis.json
  operationId: at-iva-sa-autoridade-tributária-iva-situação-atual
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

<div style={{ textAlign: "center" }}>
  <h3>DOWNLOAD PROJECT</h3>
</div>

- [Java](https://we.tl/t-7pBtGcvBI6)
- [Python](https://we.tl/t-4x2DgpxZW8)
- [C#](https://we.tl/t-pF7tBODm8W)

<a href="https://www.bizapis.com/wp-content/uploads/2024/08/at-iva-sa.mp4.mp4" target="_blank">
  To watch the video click here
</a>

# JSON Schema API Response

## Portuguese

```json
{
  "type" : "object",
  "properties" : {
    "RequestId" : {
      "type" : "string",
      "description" : "Identificador único do pedido."
    },
    "ivaList" : {
      "type" : "object",
      "description" : "Lista dos períodos de tributação do IVA, organizados por período.",
      "additionalProperties" : {
        "type" : "array",
        "items" : {
          "type" : "object",
          "properties" : {
            "periodo" : {
              "type" : "string",
              "description" : "Período de tributação em formato 'YYMM'. Representa o ano e o mês do imposto."
            },
            "entregues" : {
              "type" : "string",
              "description" : "Número de declarações periódicas entregues para o período."
            },
            "emFalta" : {
              "type" : "string",
              "description" : "Número de declarações periódicas que não foram entregues para o período."
            },
            "reembolsoPedido" : {
              "type" : "string",
              "description" : "Número de pedidos de reembolso realizados para o período."
            },
            "reembolsoEmAnalise" : {
              "type" : "string",
              "description" : "Número de pedidos de reembolso que estão em análise para o período."
            },
            "reembolsoDeferido" : {
              "type" : "string",
              "description" : "Número de pedidos de reembolso que foram deferidos para o período."
            },
            "declaracaoRecapit" : {
              "type" : "string",
              "description" : "Número de declarações recapitulativas associadas ao período."
            }
          }
        }
      }
    }
  }
}
```

## English

```json
{
  "type": "object",
  "properties": {
    "RequestId": {
      "type": "string",
      "description": "Unique identifier for the request."
    },
    "ivaList": {
      "type": "object",
      "description": "List of VAT taxation periods, organized by period.",
      "additionalProperties": {
        "type": "array",
        "items": {
          "type": "object",
          "properties": {
            "periodo": {
              "type": "string",
              "description": "Taxation period in the format 'YYMM'. Represents the year and month of the tax."
            },
            "entregues": {
              "type": "string",
              "description": "Number of periodic declarations submitted for the period."
            },
            "emFalta": {
              "type": "string",
              "description": "Number of periodic declarations that were not submitted for the period."
            },
            "reembolsoPedido": {
              "type": "string",
              "description": "Number of refund requests made for the period."
            },
            "reembolsoEmAnalise": {
              "type": "string",
              "description": "Number of refund requests under analysis for the period."
            },
            "reembolsoDeferido": {
              "type": "string",
              "description": "Number of refund requests that have been approved for the period."
            },
            "declaracaoRecapit": {
              "type": "string",
              "description": "Number of recapitulative declarations associated with the period."
            }
          }
        }
      }
    }
  }
}
```