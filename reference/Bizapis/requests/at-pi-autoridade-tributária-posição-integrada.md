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
# Download Project

<div style={{ textAlign: "center" }}>
  <h3>DOWNLOAD PROJECT</h3>
</div>

- [Java](https://go.wetransfer.com/t-MVh3FFDQMU)
- [Python](https://go.wetransfer.com/t-tV4gdzCgMj)
- [C#](https://go.wetransfer.com/t-RzDzmvAuFi)

{/* <a href="https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download">
  <button>Download project demo</button>
</a> */}

<a href="https://www.bizapis.com/wp-content/uploads/2024/08/autoridade_tributaria_posicao_integrada.mp4.mp4" target="_blank">
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

## English

```json
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