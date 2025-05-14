---
title: AT-IVA-DP (Autoridade Tributária IVA Declarações Periódicas)
excerpt: >-
  Endpoint to retrieve the list of IVA (Imposto sobre Valor Acrescentado
  Declaração periódica) in Autoridade Tributária.
api:
  file: bizapis.json
  operationId: at-iva-dp-autoridade-tributária-iva-declarações-periódicas
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
>   <li><a href="https://we.tl/t-amKnfmEuOF">Java</a></li>
>   <li><a href="https://we.tl/t-8C1B0mcUls">Python</a></li>
>   <li><a href="https://we.tl/t-R01JtoUQme">C#</a></li>
> </ul>
> `}</HTMLBlock>

<HTMLBlock>{`
<a href="https://www.bizapis.com/wp-content/uploads/2024/08/at-iva-dp.mp4.mp4" target="_blank">To watch the video click here</a>
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
    "results" : {
      "type" : "string",
      "description" : "Número total de resultados disponíveis na consulta."
    },
    "totalPages" : {
      "type" : "integer",
      "description" : "Número total de páginas disponíveis na consulta."
    },
    "atIvaList" : {
      "type" : "array",
      "description" : "Lista de declarações de IVA detalhadas.",
      "items" : {
        "type" : "object",
        "properties" : {
          "declaracao" : {
            "type" : "string",
            "description" : "Identificador ou referência à declaração associada ao período do IVA."
          },
          "vigente" : {
            "type" : "string",
            "description" : "Indica se a declaração está em vigor."
          },
          "periodo" : {
            "type" : "string",
            "description" : "Período de tributação do IVA no formato 'YYMM'."
          },
          "estado" : {
            "type" : "string",
            "description" : "Estado atual da declaração."
          },
          "dataSub" : {
            "type" : "string",
            "description" : "Data de submissão da declaração no formato 'AAAA-MM-DD'."
          },
          "valor" : {
            "type" : "string",
            "description" : "Valor total reportado na declaração do IVA."
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
      "description": "Unique identifier of the request."
    },
    "results": {
      "type": "string",
      "description": "Total number of results available in the query."
    },
    "totalPages": {
      "type": "integer",
      "description": "Total number of pages available in the query."
    },
    "atIvaList": {
      "type": "array",
      "description": "List of detailed VAT declarations.",
      "items": {
        "type": "object",
        "properties": {
          "declaracao": {
            "type": "string",
            "description": "Identifier or reference to the declaration associated with the VAT period."
          },
          "vigente": {
            "type": "string",
            "description": "Indicates whether the declaration is active."
          },
          "periodo": {
            "type": "string",
            "description": "VAT taxation period in the format 'YYMM'."
          },
          "estado": {
            "type": "string",
            "description": "Current status of the declaration."
          },
          "dataSub": {
            "type": "string",
            "description": "Date of submission of the declaration in the format 'YYYY-MM-DD'."
          },
          "valor": {
            "type": "string",
            "description": "Total amount reported in the VAT declaration."
          }
        }
      }
    }
  }
}
```