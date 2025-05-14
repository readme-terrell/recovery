---
title: AT-Divida (Autoridade Tributária Dívida/Não Dívida
excerpt: >-
  Endpoint to retrieve the document "Dívida/Não Dívida" from Autoridade
  Tributária
api:
  file: bizapis.json
  operationId: at-divida
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
>   <li><a href="https://we.tl/t-VngYT4lHin">Java</a></li>
>   <li><a href="https://we.tl/t-hWGL7PXd3W">Python</a></li>
>   <li><a href="https://we.tl/t-vARneSpzqv">C#</a></li>
> </ul>
> {/* 
> <a href="https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download">
>   <button>Download project demo</button>
> </a> */}
> `}</HTMLBlock>

<HTMLBlock>{`
<a href="https://www.bizapis.com/wp-content/uploads/2024/08/autoridade_tributaria_divida.mp4.mp4" target="_blank">To watch the video click here</a>
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