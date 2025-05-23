---
title: IES (Informação Empresarial Simplificada)
excerpt: This endpoint allows you to consult IES (Informação Empresarial Simplificada).
api:
  file: bizapis.json
  operationId: ies-informação-empresarial-simplificada
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

- [Java](https://we.tl/t-8U051WQwfe)
- [Python](https://we.tl/t-ynSKuElrpE)
- [C#](https://we.tl/t-4SaCPBTr7A)

[Watch the video](https://www.bizapis.com/wp-content/uploads/2024/08/seervico_informacao_empresarial_simplificada.mp4.mp4)

# JSON Schema API Response

## Portuguese (PT)

```json
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

## English (ENG)

```json
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