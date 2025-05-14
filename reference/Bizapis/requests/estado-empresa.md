---
title: Estado-Empresa (Estado da Empresa)
excerpt: >-
  The Estado-Empresais a digital document that assesses the company's status.
  This endpoint allows you to consult Publicações de Atos Societários e de
  outras entidades.
api:
  file: bizapis.json
  operationId: estado-empresa
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
>   <li><a href="https://we.tl/t-p1fCQBEkCa">Java</a></li>
>   <li><a href="https://we.tl/t-m1mQjCzMM7">Python</a></li>
>   <li><a href="https://we.tl/t-qicLCvyYzh">C#</a></li>
> </ul>
> {/* <a href="https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download">
>   <button>Download project demo</button>
> </a> */}
> `}</HTMLBlock>

<HTMLBlock>{`
<a href="https://www.bizapis.com/wp-content/uploads/2024/08/estado-empresa.mp4.mp4" target="_blank">To watch the video click here</a>
`}</HTMLBlock>

# JSON Schema API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "RequestId" : {
      "type" : "string",
      "description" : "Identificador único do pedido."
    },
    "Date" : {
      "type" : "string",
      "description" : "Data da publicação do ato ou facto (formato: YYYY-MM-DD)."
    },
    "NIPC" : {
      "type" : "string",
      "description" : "Número de Identificação de Pessoa Coletiva (NIPC) da entidade."
    },
    "Entity" : {
      "type" : "string",
      "description" : "Nome da entidade associada."
    },
    "County" : {
      "type" : "string",
      "description" : "Concelho onde a entidade está localizada."
    },
    "Act/Fact" : {
      "type" : "string",
      "description" : "Descrição do ato ou facto publicado."
    },
    "Status" : {
      "type" : "string",
      "description" : "Estado atual da entidade."
    },
    "Code" : {
      "type" : "string",
      "description" : "Código associado ao tipo de Act/Fact."
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
    "Date": {
      "type": "string",
      "description": "Date of the publication of the act or fact (format: YYYY-MM-DD)."
    },
    "NIPC": {
      "type": "string",
      "description": "Corporate Taxpayer Identification Number (NIPC) of the entity."
    },
    "Entity": {
      "type": "string",
      "description": "Name of the associated entity."
    },
    "County": {
      "type": "string",
      "description": "County where the entity is located."
    },
    "Act/Fact": {
      "type": "string",
      "description": "Description of the published act or fact."
    },
    "Status": {
      "type": "string",
      "description": "Current status of the entity."
    },
    "Code": {
      "type": "string",
      "description": "Code associated with the type of Act/Fact."
    }
  }
}
```