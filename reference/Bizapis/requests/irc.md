---
title: AT-IRC (Autoridade Tributária-Imposto Sobre o Rendimento)
excerpt: >-
  Endpoint to retrieve the list of IRC (Imposto sobre o Rendimento das Pessoas
  Coletivas) in Autoridade Tributária.
api:
  file: bizapis.json
  operationId: irc
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
> [block:html]{"html":"<h3  style=\"text-align:center;\">DOWNLOAD PROJECT</h3>\n<ul>\n  <li><a href=\"https://go.wetransfer.com/t-e7cxf83lLd\">Java</li>\n  <li><a href=\"https://go.wetransfer.com/t-6s26J2Akft\">Python</li>\n  <li><a href=\"https://go.wetransfer.com/t-6BfF8vtkpx\">C#</li>\n</ul>\n<!--\n<a href=\"https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download\">\n  <button>Download project demo</button>\n</a> -->"}[/block]

[block:html]
{
  "html": "<a href=\"https://www.bizapis.com/wp-content/uploads/2024/08/autoridade_tributaria_irc.mp4.mp4\" target=\"_blank\">To watch the video click here"
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
    "alert" : {
      "type" : "string",
      "description" : "Mensagem de alerta emitida pela Autoridade Tributária. Pode incluir informações como prazos ou obrigações fiscais."
    },
    "list" : {
      "type" : "array",
      "description" : "Lista de registos fiscais relacionados com o Imposto sobre o Rendimento de Pessoas Coletivas (IRC), incluindo ano, situação e data.",
      "items" : {
        "type" : "object",
        "properties" : {
          "year" : {
            "type" : "string",
            "description" : "Ano em observação."
          },
          "situation" : {
            "type" : "string",
            "description" : "Situação fiscal para o ano especificado."
          },
          "date" : {
            "type" : "string",
            "description" : "Data em que a situação foi determinada ou registada, no formato 'YYYY-MM-DD'."
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
    "alert": {
      "type": "string",
      "description": "Alert message issued by the Tax Authority. May include information such as deadlines or tax obligations."
    },
    "list": {
      "type": "array",
      "description": "List of tax records related to the Corporate Income Tax (IRC), including year, situation, and date.",
      "items": {
        "type": "object",
        "properties": {
          "year": {
            "type": "string",
            "description": "Year under observation."
          },
          "situation": {
            "type": "string",
            "description": "Tax situation for the specified year."
          },
          "date": {
            "type": "string",
            "description": "Date when the situation was determined or registered, in the format 'YYYY-MM-DD'."
          }
        }
      }
    }
  }
}

```