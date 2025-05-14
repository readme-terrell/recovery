---
title: CE (Certificados Energéticos)
excerpt: >-
  The CE is a digital document that evaluates the energy performance of a home.
  This endpoint permits the consult of energy certificates.
api:
  file: bizapis.json
  operationId: ce-certificados-energéticos
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
>   <li><a href="https://we.tl/t-bIZoRJjUhC">Java</a></li>
>   <li><a href="https://we.tl/t-DSxaFgrUeE">Python</a></li>
>   <li><a href="https://we.tl/t-uz0C3JLPXM">C#</a></li>
> </ul>
> {/* <a href="https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download">
>   <button>Download project demo</button>
> </a> */}
> `}</HTMLBlock>

<HTMLBlock>{`
<a href="https://www.bizapis.com/wp-content/uploads/2024/08/servico_certificados_energeticos.mp4.mp4" target="_blank">To watch the video click here</a>
`}</HTMLBlock>

# JSON Schema API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "RequestId" : {
      "type" : "string"
    },
    "EnergyCertificates" : {
      "type" : "array",
      "description" : "Lista de certificados energéticos",
      "items" : {
        "type" : "object",
        "properties" : {
          "TituloDocumento" : {
            "type" : "string",
            "description" : "Título do documento"
          },
          "RequestId" : {
            "type" : "string",
            "description" : "Identificador único do pedido"
          },
          "NumDocumento" : {
            "type" : "string",
            "description" : "Identificador do documento"
          },
          "TipoDocumento" : {
            "type" : "string",
            "description" : "Tipo de documento"
          },
          "Morada" : {
            "type" : "string",
            "description" : "Morada do imóvel"
          },
          "Localidade" : {
            "type" : "string",
            "description" : "Localidade do imóvel"
          },
          "Freguesia" : {
            "type" : "string",
            "description" : "Freguesia do imóvel"
          },
          "Concelho" : {
            "type" : "string",
            "description" : "Concelho do imóvel"
          },
          "DataEmissao" : {
            "type" : "string",
            "description" : "Data de emissão do documento"
          },
          "DataValidade" : {
            "type" : "string",
            "description" : "Data de validade do documento"
          },
          "NumPeritoQualificado" : {
            "type" : "string",
            "description" : "Identificador do perito qualificado"
          },
          "ClasseEnergetica" : {
            "type" : "string",
            "description" : "Classe energética do imóvel"
          },
          "ArtigoMatricial" : {
            "type" : "string",
            "description" : "Artigo matricial do imóvel"
          },
          "Conservatoria" : {
            "type" : "string",
            "description" : "Conservatória do Registo Predial"
          },
          "NumConservatoria" : {
            "type" : "string",
            "description" : "Número da Conservatória do Registo Predial"
          },
          "FracaoAutonoma" : {
            "type" : "string",
            "description" : "Fração autónoma do imóvel"
          },
          "Similaridade" : {
            "type" : "number",
            "description" : "Similaridade entre os campos de resposta e os campos de pesquisa"
          }
        }
      }
    },
    "NumResultados" : {
      "type" : "integer",
      "description" : "Número de resultados encontrados"
    }
  }
}
```
```json ENG
{
  "type": "object",
  "properties": {
    "RequestId": {
      "type": "string"
    },
    "EnergyCertificates": {
      "type": "array",
      "description": "List of energy certificates",
      "items": {
        "type": "object",
        "properties": {
          "TituloDocumento": {
            "type": "string",
            "description": "Document title"
          },
          "RequestId": {
            "type": "string",
            "description": "Unique request identifier"
          },
          "NumDocumento": {
            "type": "string",
            "description": "Document identifier"
          },
          "TipoDocumento": {
            "type": "string",
            "description": "Document type"
          },
          "Morada": {
            "type": "string",
            "description": "Property address"
          },
          "Localidade": {
            "type": "string",
            "description": "Property locality"
          },
          "Freguesia": {
            "type": "string",
            "description": "Property parish"
          },
          "Concelho": {
            "type": "string",
            "description": "Property municipality"
          },
          "DataEmissao": {
            "type": "string",
            "description": "Document issue date"
          },
          "DataValidade": {
            "type": "string",
            "description": "Document expiration date"
          },
          "NumPeritoQualificado": {
            "type": "string",
            "description": "Qualified expert identifier"
          },
          "ClasseEnergetica": {
            "type": "string",
            "description": "Property energy class"
          },
          "ArtigoMatricial": {
            "type": "string",
            "description": "Property registration number"
          },
          "Conservatoria": {
            "type": "string",
            "description": "Land Registry Office"
          },
          "NumConservatoria": {
            "type": "string",
            "description": "Land Registry Office number"
          },
          "FracaoAutonoma": {
            "type": "string",
            "description": "Property autonomous fraction"
          },
          "Similaridade": {
            "type": "number",
            "description": "Similarity between response fields and search fields"
          }
        }
      }
    },
    "NumResultados": {
      "type": "integer",
      "description": "Number of results found"
    }
  }
}
```