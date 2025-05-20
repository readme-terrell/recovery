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
# Download Project

<div style={{ textAlign: "center" }}>
  <h3>DOWNLOAD PROJECT</h3>
</div>

- [Java](https://we.tl/t-VngYT4lHin)
- [Python](https://we.tl/t-hWGL7PXd3W)
- [C#](https://we.tl/t-vARneSpzqv)

{/* 
<a href="https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download">
  <button>Download project demo</button>
</a> 
*/}

<a href="https://www.bizapis.com/wp-content/uploads/2024/08/autoridade_tributaria_divida.mp4.mp4" target="_blank">
  To watch the video click here
</a>

# JSON Schema API Response

## Portuguese

```json
{
  "type": "object",
  "properties": {
    "data": {
      "type": "object",
      "properties": {
        "requestId": {
          "type": "string",
          "description": "Identificador único do pedido"
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

## English

```json
{
  "type": "object",
  "properties": {
    "data": {
      "type": "object",
      "properties": {
        "requestId": {
          "type": "string",
          "description": "Unique request identifier"
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