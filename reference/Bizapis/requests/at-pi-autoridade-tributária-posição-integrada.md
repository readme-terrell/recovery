---
title: AT-PI (Autoridade Tributária Posição Integrada)
excerpt: >-
  Endpoint to retrieve the values corresponding to Posição Integrada in
  Autoridade Tributária.
api:
  file: bizapis.json
  operationId: at-pi-autoridade-tributária-posição-integrada
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
> 💻 [block:html]{"html":"<h3  style=\"text-align:center;\">DOWNLOAD PROJECT</h3>\n<ul>\n  <li><a href=\"https://go.wetransfer.com/t-MVh3FFDQMU\">Java</li>\n  <li><a href=\"https://go.wetransfer.com/t-tV4gdzCgMj\">Python</li>\n  <li><a href=\"https://go.wetransfer.com/t-RzDzmvAuFi\">C#</li>\n</ul>\n<!--\n<a href=\"https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download\">\n  <button>Download project demo</button>\n</a> -->"}[/block]

[block:html]
{
  "html": "<a href=\"https://www.bizapis.com/wp-content/uploads/2024/08/autoridade_tributaria_posicao_integrada.mp4.mp4\" target=\"_blank\">To watch the video click here"
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
    "atpiList" : {  
      "type" : "array",  
      "description" : "Informações consolidadas sobre a posição integrada do contribuinte na Autoridade Tributária.",  
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
    "atpiList": {
      "type": "array",
      "description": "Consolidated information about the taxpayer's integrated position with the Tax Authority.",
      "items": {
        "type": "object",
        "properties": {
          "title": {
            "type": "string",
            "description": "The title that represents the specific tax item."
          },
          "status": {
            "type": "string",
            "description": "The current state of the item. 'Green' means 'compliance', 'Yellow' means 'in progress', and 'Red' means 'non-compliance'."
          }
        }
      }
    }
  }
}

```