---
title: Debt (Dívidas Autoridade Tributária/Segurança Social)
excerpt: >-
  Endpoint to identify if a person is currently in debt to Segurança Social or
  Autoridade Tributária.It takes the persons NIF and the portal that could
  assume the values "AT" (Autoridade Tributária) or "SS" (Segurança Social) as
  inputs
api:
  file: bizapis.json
  operationId: debt
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
>   <li><a href="https://we.tl/t-LoKh0HSmDx">Java</a></li>
>   <li><a href="https://we.tl/t-flFrxOTJLK">Python</a></li>
>   <li><a href="https://we.tl/t-amS0lzmLaL">C#</a></li>
> </ul>
> `}</HTMLBlock>

<HTMLBlock>{`
<a href="https://www.bizapis.com/wp-content/uploads/2024/08/servico_debt.mp4.mp4" target="_blank">To watch the video click here</a>
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
    "NIF" : {
      "type" : "string",
      "description" : "Número de Identificação Fiscal (NIF) da entidade ou do indivíduo."
    },
    "Name" : {
      "type" : "string",
      "description" : "Nome completo da entidade ou do indivíduo."
    },
    "Last update" : {
      "type" : "string",
      "description" : "Data e hora da última atualização do registo (formato: YYYY-MM-DD)."
    },
    "TierValueGreaterThan" : {
      "type" : "integer",
      "description" : "Valor mínimo para filtrar os registos. Apenas registos com um valor superior a este número serão incluídos."
    },
    "TierValueLessThan" : {
      "type" : "integer",
      "description" : "Valor máximo para filtrar os registos. Apenas registos com um valor inferior a este número serão incluídos."
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
      "description": "A unique identifier for the request."
    },
    "NIF": {
      "type": "string",
      "description": "The Tax Identification Number (NIF) of the entity or individual."
    },
    "Name": {
      "type": "string",
      "description": "The full name of the entity or individual."
    },
    "Last update": {
      "type": "string",
      "description": "The date and time when the record was last updated (format: DD/MM/YYYY HH:mm)."
    },
    "TierValueGreaterThan": {
      "type": "integer",
      "description": "The minimum tier value for filtering records. Only records with a tier value greater than this number will be included."
    },
    "TierValueLessThan": {
      "type": "integer",
      "description": "The maximum tier value for filtering records. Only records with a tier value less than this number will be included."
    }
  }
}
```