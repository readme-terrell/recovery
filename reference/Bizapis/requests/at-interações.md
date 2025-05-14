---
title: AT-Interações (Autoridade Tributária - Interações)
excerpt: Endpoint to retrieve list of "Interações" present in Autoridade Tributária
api:
  file: bizapis.json
  operationId: at-interações
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
> 🖥️ [block:html]{"html":"<h3  style=\"text-align:center;\">DOWNLOAD PROJECT</h3>\n<ul>\n  <li><a href=\"https://we.tl/t-bj6hrkWc4V\">Java</li>\n  <li><a href=\"https://we.tl/t-k8X5hEXFic\">Python</li>\n  <li><a href=\"https://we.tl/t-chJYI59QbM\">C#</li>\n</ul>\n<!--\n<a href=\"https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download\">\n  <button>Download project demo</button>\n</a> -->"}[/block]

[block:html]
{
  "html": "<a href=\"https://www.bizapis.com/wp-content/uploads/2024/08/servico_autoridade_tributaria_interacoes.mp4.mp4\" target=\"_blank\">To watch the video click here"
}
[/block]


# JSON Schema API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "RequestId" : {
      "type" : "string",
      "description" : "Identificador único do pedido."
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
      "type": "string",
      "description": "Unique identifier for the request."
    },
    "Interacoes": {
      "type": "array",
      "description": "Record of interactions between the taxpayer and the Tax Authority, including submissions, information requests, and AT responses.",
      "items": {
        "type": "object",
        "properties": {
          "tax": {
            "type": "string",
            "description": "The type of tax or fiscal item related to this interaction."
          },
          "description": {
            "type": "string",
            "description": "A detailed description of the interaction, such as its purpose or context."
          },
          "date": {
            "type": "string",
            "description": "The date the interaction occurred, in the format 'YYYY-MM-DD'."
          }
        }
      }
    }
  }
}

```