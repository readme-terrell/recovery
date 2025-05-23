---
title: NifName  (Número Fiscal e Nome)
excerpt: This endpoint allows querying the NIF and the associated name.
api:
  file: bizapis.json
  operationId: nifname
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

- [Java](https://we.tl/t-ltawfTIv5s)
- [Python](https://we.tl/t-Wza4cCzjuK)
- [C#](https://we.tl/t-4HmOfN9uKG)

[Watch the video](https://www.bizapis.com/wp-content/uploads/2024/08/nifname.mp4.mp4)

# JSON Schema for API Response

## Portuguese (PT)

```json
{
  "type": "object",
  "properties": {
    "nif": {
      "type": "string",
      "description": "Número Identificação Fiscal"
    },
    "name": {
      "type": "string",
      "description": "Nome"
    },
    "cod_financas": {
      "type": "string",
      "description": "Dados do Serviço Finanças - Código"
    },
    "desc_financas": {
      "type": "string",
      "description": "Dados do Serviço Finanças - Descrição"
    },
    "act_css_iva": {
      "type": "string",
      "description": "Dados de Atividade - Data de Cessação do Imposto sobre Valor Acrescentado (IVA)"
    },
    "act_css_irs": {
      "type": "string",
      "description": "Dados de Atividade - Data de Cessação do Imposto sobre o Rendimento das Pessoas Singulares (IRS)"
    },
    "inclusion_iva": {
      "type": "string",
      "description": "Dados de Atividade - Enquadramento Imposto sobre Valor Acrescentado (IVA)"
    },
    "situation": {
      "type": "string",
      "description": "Dados de Atividade - Situação"
    },
    "activity_message": {
      "type": "string",
      "description": "Mensagem para quando não existe atividade"
    }
  }
}
```

## English (ENG)

```json
{
  "type": "object",
  "properties": {
    "nif": {
      "type": "string",
      "description": "Tax Identification Number (NIF)"
    },
    "name": {
      "type": "string",
      "description": "Full Name of the Entity or Individual"
    },
    "cod_financas": {
      "type": "string",
      "description": "Tax Office Code"
    },
    "desc_financas": {
      "type": "string",
      "description": "Tax Office Description"
    },
    "act_css_iva": {
      "type": "string",
      "description": "Date of VAT (Value Added Tax) Termination"
    },
    "act_css_irs": {
      "type": "string",
      "description": "Date of Income Tax Termination"
    },
    "inclusion_iva": {
      "type": "string",
      "description": "VAT (Value Added Tax) Framework Details"
    },
    "situation": {
      "type": "string",
      "description": "Current Activity Status"
    },
    "activity_message": {
      "type": "string",
      "description": "Message for Non-Activity Status"
    }
  }
}
```