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
> 💻 [block:html]{"html":"<h3  style=\"text-align:center;\">DOWNLOAD PROJECT</h3>\n<ul>\n  <li><a href=\"https://we.tl/t-ltawfTIv5s\">Java</li>\n  <li><a href=\"https://we.tl/t-Wza4cCzjuK\">Python</li>\n  <li><a href=\"https://we.tl/t-4HmOfN9uKG\">C#</li>\n</ul>\n<!--\n<a href=\"https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download\">\n  <button>Download project demo</button>\n</a> -->"}[/block]

[block:html]
{
  "html": "<a href=\"https://www.bizapis.com/wp-content/uploads/2024/08/nifname.mp4.mp4\" target=\"_blank\">To watch the video click here"
}
[/block]


# JSON Schema for API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "nif" : {
      "type" : "string",
      "description" : "Número Identificação Fiscal"
    },
    "name" : {
      "type" : "string",
      "description" : "Nome"
    },
    "cod_financas" : {
      "type" : "string",
      "description" : "Dados do Serviço Finanças - Código"
    },
    "desc_financas" : {
      "type" : "string",
      "description" : "Dados do Serviço Finanças - Descrição"
    },
    "act_css_iva" : {
      "type" : "string",
      "description" : "Dados de Atividade - Data de Cessação do Imposto sobre Valor Acrescentado (IVA)"
    },
    "act_css_irs" : {
      "type" : "string",
      "description" : "Dados de Atividade - Data de Cessação do Imposto sobre o Rendimento das Pessoas Singulares (IRS)"
    },
    "inclusion_iva" : {
      "type" : "string",
      "description" : "Dados de Atividade - Enquadramento Imposto sobre Valor Acrescentado (IVA)"
    },
    "situation" : {
      "type" : "string",
      "description" : "Dados de Atividade - Situação"
    },
    "activity_message" : {
      "type" : "string",
      "description" : "Mensagem para quando não existe atividade"
    }
  }
}
```
```json ENG
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