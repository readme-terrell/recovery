---
title: AT-Aggregator (Autoridade Tributária Agregador)
excerpt: >-
  Retrieve information about the current alerts, interactions and the integrated
  position from Autoridade Tributária
api:
  file: bizapis.json
  operationId: at-aggregator
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
> 💻
>
> <HTMLBlock>{`
> <h3  style="text-align:center;">DOWNLOAD PROJECT</h3>
> <ul>
>   <li><a href="https://we.tl/t-j1sps7Yh6S" target="_blank">Java</li>
>   <li><a href="https://we.tl/t-sKPJdG7PCN">Python</li>
>   <li><a href="https://we.tl/t-2cTl7XiWZZ">C#</li>
> </ul>
> <!--
> <a href="https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download">
>   <button>Download project demo</button>
> </a> -->
> `}</HTMLBlock>

<HTMLBlock>{`
<a href="https://www.bizapis.com/wp-content/uploads/2024/08/autoridade_tributaria_aggregator.mp4.mp4" target="_blank">To watch the video click here
`}</HTMLBlock>

# JSON Schema for API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "RequestId" : {
      "type" : "string"
    },
    "Posicao Integrada" : {
      "type" : "array",
      "description" : "Informações consolidadas sobre a posição integrada do contribuinte junto à Autoridade Tributária.",
      "items" : {
        "type" : "object",
        "properties" : {
          "title" : {
            "type" : "string",
            "description" : "O título que representa o item fiscal específico."
          },
          "status" : {
            "type" : "string",
            "description" : "O estado atual do item. 'Verde' significa 'cumprimento', 'Amarelo' significa 'em progresso' e 'Vermelho' significa 'incumprimento'."
          }
        }
      }
    },
    "Alertas" : {
      "type" : "array",
      "description" : "Lista de alertas emitidos pela Autoridade Tributária. Pode incluir prazos de pagamento, avisos de irregularidades ou necessidade de submissão de declarações.",
      "items" : {
        "type" : "object",
        "properties" : {
          "descriptionName" : {
            "type" : "string",
            "description" : "O nome ou categoria do alerta."
          },
          "description" : {
            "type" : "string",
            "description" : "Uma explicação detalhada sobre o alerta."
          },
          "limitDate" : {
            "type" : "string",
            "description" : "O prazo ou data em que a ação associada ao alerta deve ser concluída, no formato 'YYYY-MM-DD'."
          }
        }
      }
    },
    "Interacoes" : {
      "type" : "array",
      "description" : "Registro de interações entre o contribuinte e a Autoridade Tributária, incluindo submissões, pedidos de informação e respostas da AT.",
      "items" : {
        "type" : "object",
        "properties" : {
          "tax" : {
            "type" : "string",
            "description" : "O tipo de imposto ou item fiscal relacionado com esta interação."
          },
          "description" : {
            "type" : "string",
            "description" : "Uma descrição detalhada da interação, como o propósito ou contexto."
          },
          "date" : {
            "type" : "string",
            "description" : "A data em que a interação ocorreu, no formato 'YYYY-MM-DD'."
          }
        }
      }
    }
  }
}
```
```json ENG
{
  "type": "object",
  "properties": {
    "RequestId": {
      "type": "string"
    },
    "Posicao Integrada": {
      "type": "array",
      "description": "Consolidated information about the taxpayer's fiscal position with the Tax Authority.",
      "items": {
        "type": "object",
        "properties": {
          "title": {
            "type": "string",
            "description": "The title or header representing the specific tax-related item."
          },
          "status": {
            "type": "string",
            "description": "The current status of the item. 'Green' means 'in compliance', 'Yellow' means 'in progress', and 'Red' means 'non-compliance'."
          }
        }
      }
    },
    "Alertas": {
      "type": "array",
      "description": "List of alerts issued by the Tax Authority. May include payment deadlines, irregularity notices, or the need to submit declarations.",
      "items": {
        "type": "object",
        "properties": {
          "descriptionName": {
            "type": "string",
            "description": "The name or category of the alert."
          },
          "description": {
            "type": "string",
            "description": "A detailed explanation of the alert."
          },
          "limitDate": {
            "type": "string",
            "description": "The deadline or date by which the action associated with this alert must be taken, formatted as 'YYYY-MM-DD'."
          }
        }
      }
    },
    "Interacoes": {
      "type": "array",
      "description": "Record of interactions between the taxpayer and the Tax Authority, including submissions, information requests, and responses from the Tax Authority.",
      "items": {
        "type": "object",
        "properties": {
          "tax": {
            "type": "string",
            "description": "The type of tax or fiscal item related to this interaction."
          },
          "description": {
            "type": "string",
            "description": "A detailed description of the interaction, such as the purpose or context."
          },
          "date": {
            "type": "string",
            "description": "The date when the interaction occurred, formatted as 'YYYY-MM-DD'."
          }
        }
      }
    }
  }
}
```
