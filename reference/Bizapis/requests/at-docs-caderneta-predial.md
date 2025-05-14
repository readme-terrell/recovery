---
title: CP (Caderneta Predial)
excerpt: >-
  The building book is a document that contains all relevant information about
  the property. This endpoint retrieves this document in an encoded base64 pdf.
api:
  file: bizapis.json
  operationId: at-docs-caderneta-predial
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
> 💻 <HTMLBlock>{`
> <h3 style={{ textAlign: "center" }}>DOWNLOAD PROJECT</h3>
> <ul>
>   <li><a href="https://we.tl/t-J5OYyufHwX">Java</a></li>
>   <li><a href="https://we.tl/t-EzgeiuzAiC">Python</a></li>
>   <li><a href="https://we.tl/t-nHdO5uyGS9">C#</a></li>
> </ul>
> {/* 
> <a href="https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download">
>   <button>Download project demo</button>
> </a> */}
> `}</HTMLBlock>

<HTMLBlock>{`
<a href="https://www.bizapis.com/wp-content/uploads/2024/08/servico_caderneta_predial.mp4.mp4" target="_blank">To watch the video click here</a>
`}</HTMLBlock>

# JSON Schema API Response

```json PT
{
  "type": "object",
  "properties": {
    "data": {
      "type": "object",
      "properties": {
        "requestId" : {
          "type" : "string",
          "description" : "Identificador único do pedido"
        }
      }
    },
    "file": {
      "type": "string",
      "description": "Ficheiro PDF em base 64"
    }
  }
}

```
```json ENG
{
  "type": "object",
  "properties": {
    "data": {
      "type": "object",
      "properties": {
        "requestId" : {
          "type" : "string",
          "description" : "Unique request identifier"
        }
      }
    },
    "file": {
      "type": "string",
      "description": "Encoded base 64 file."
    }
  }
}

```