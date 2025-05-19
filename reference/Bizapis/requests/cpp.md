---
title: CPP (Certidão Permanente Predial)
excerpt: >-
  The permanent property certificate is a digital document with all records
  about a property. With this endpoint it's possible to obtain the document in
  encoded base64.
api:
  file: bizapis.json
  operationId: cpp
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
>   <li><a href="https://we.tl/t-nXjAbUKfYI">Java</li>
>   <li><a href="https://we.tl/t-WMm2XLQG3z">Python</li>
>   <li><a href="https://we.tl/t-4tmj2arQgi">C#</li>
> </ul>
> <!--
> <a href="https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download">
>   <button>Download project demo</button>
> </a> -->
> `}</HTMLBlock>

<HTMLBlock>{`
<a href="https://www.bizapis.com/wp-content/uploads/2024/08/servico_certidao_permanente_predial.mp4.mp4" target="_blank">To watch the video click here
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