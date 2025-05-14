---
title: AT-IVA-Enquadramento (Autoridade Tributária Enquadramento do IVA)
excerpt: >-
  Endpoint to retrieve the list of IVA (Imposto sobre Valor Acrescentado
  Enquadramento) in Autoridade Tributária.
api:
  file: bizapis.json
  operationId: at-iva-enquadramento-autoridade-tributária-enquadramento-do-iva
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
> 💻 [block:html]{"html":"<h3  style=\"text-align:center;\">DOWNLOAD PROJECT</h3>\n<ul>\n  <li><a href=\"https://we.tl/t-0oUrpIaP0K\">Java</li>\n  <li><a href=\"https://we.tl/t-UMlRtF7Quu\">Python</li>\n  <li><a href=\"https://we.tl/t-6MX8ko14rW\">C#</li>\n</ul>\n<!--\n<a href=\"https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download\">\n  <button>Download project demo</button>\n</a> -->"}[/block]

[block:html]
{
  "html": "<a href=\"https://www.bizapis.com/wp-content/uploads/2024/08/autoridade_tributaria_iva_enquadramento-2.mp4.mp4\" target=\"_blank\">To watch the video click here"
}
[/block]


# Json Schema API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "RequestId" : {
      "type" : "string",
      "description" : "Identificador único do pedido."
    },
    "enquadramento" : {
      "type" : "string",
      "description" : "Tipo de enquadramento do contribuinte para efeitos de Imposto sobre Valor Acrescentado."
    },
    "dataDeEnquadramento" : {
      "type" : "string",
      "description" : "Data de início do enquadramento do contribuinte no regime de Imposto sobre Valor Acrescentado."
    },
    "situacao" : {
      "type" : "string",
      "description" : "Situação atual do enquadramento fiscal do contribuinte."
    },
    "dataDeCessao" : {
      "type" : "string",
      "description" : "Data em que o enquadramento foi cessado, caso aplicável."
    },
    "motivoDeCessao" : {
      "type" : "string",
      "description" : "Motivo da cessação do enquadramento fiscal."
    },
    "nifDaCaessao" : {
      "type" : "string",
      "description" : "Número de Identificação Fiscal (NIF) do cessionário, caso aplicável."
    },
    "nomeDoCessionario" : {
      "type" : "string",
      "description" : "Nome do cessionário relacionado com a cessão de atividade, caso aplicável."
    },
    "atividadeConstante" : {
      "type" : "string",
      "description" : "Indica se exerce atividade constante."
    },
    "descricao" : {
      "type" : "string",
      "description" : "Descrição do regime especial."
    },
    "tipoOperacoes" : {
      "type" : "string",
      "description" : "Tipo de operações realizadas pelo contribuinte."
    },
    "proRataDeducaoIva" : {
      "type" : "string",
      "description" : "Pro Rata de dedução do Imposto sobre Valor Acrescentado aplicado ao contribuinte."
    },
    "transacaoIntracomunitariasBens" : {
      "type" : "string",
      "description" : "Indica se o contribuinte realiza transações intracomunitárias de bens."
    },
    "opcaoRenuncia" : {
      "type" : "string",
      "description" : "Opção de renúncia à isenção em operações Imobiliárias."
    },
    "opcaoRegime" : {
      "type" : "string",
      "description" : "Opção por regime de Tributação."
    },
    "opcaoPeriodicidade" : {
      "type" : "string",
      "description" : "Opção por Periodicidade Mensal."
    },
    "prestacao" : {
      "type" : "string",
      "description" : "Prestação/Aquisição de Serviços Intracomunitários."
    },
    "importacoes" : {
      "type" : "string",
      "description" : "Importações."
    },
    "exportacoes" : {
      "type" : "string",
      "description" : "Exportações."
    },
    "aquisicoes" : {
      "type" : "string",
      "description" : "Transações Intracomunitárias - Aquisições."
    },
    "trasnmissoes" : {
      "type" : "string",
      "description" : "Transações Intracomunitárias - Transmissões."
    },
    "reembolsoSituacao" : {
      "type" : "string",
      "description" : "Situação atual de reembolso mensal de Imposto sobre Valor Acrescentado do contribuinte."
    },
    "reembolsoDataInicio" : {
      "type" : "string",
      "description" : "Data de início do período relacionado com o reembolso de Imposto sobre Valor Acrescentado."
    },
    "reembolsoDataFim" : {
      "type" : "string",
      "description" : "Data de fim do período relacionado com o reembolso de Imposto sobre Valor Acrescentado."
    },
    "ivaDataInicio" : {
      "type" : "string",
      "description" : "Data de início do regime de Imposto sobre Valor Acrescentado de Caixa."
    },
    "ivaDataFim" : {
      "type" : "string",
      "description" : "Data de fim do regime de Imposto sobre Valor Acrescentado de Caixa."
    },
    "ivaMotivo" : {
      "type" : "string",
      "description" : "Motivo relacionado com a exclusão do regime de Imposto sobre Valor Acrescentado de Caixa."
    },
    "importacoesDataInicio" : {
      "type" : "string",
      "description" : "Data de início do período de importações, opção pelo Pagamento do Imposto na Declaração Periódica do Imposto sobre Valor Acrescentado."
    },
    "importacoesDataFim" : {
      "type" : "string",
      "description" : "Data de fim do período de importações, opção pelo Pagamento do Imposto na Declaração Periódica do Imposto sobre Valor Acrescentado."
    },
    "importacoesMotivo" : {
      "type" : "string",
      "description" : "Motivo relacionado com o cancelamento da opção pelo Pagamento do Imposto na Declaração Periódica do Imposto sobre Valor Acrescentado."
    },
    "forfetarioDataInicio" : {
      "type" : "string",
      "description" : "Data de início do regime forfetário, caso aplicável."
    },
    "forfetarioDataFim" : {
      "type" : "string",
      "description" : "Data de fim do regime forfetário, caso aplicável."
    },
    "forfetarioMotivo" : {
      "type" : "string",
      "description" : "Motivo relacionado com a aplicação do regime forfetário."
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
    "enquadramento": {
      "type": "string",
      "description": "Taxpayer's VAT regime classification."
    },
    "dataDeEnquadramento": {
      "type": "string",
      "description": "Start date of the taxpayer's VAT regime classification."
    },
    "situacao": {
      "type": "string",
      "description": "Current status of the taxpayer's fiscal classification."
    },
    "dataDeCessao": {
      "type": "string",
      "description": "Date when the taxpayer's VAT regime was terminated, if applicable."
    },
    "motivoDeCessao": {
      "type": "string",
      "description": "Reason for terminating the taxpayer's VAT regime."
    },
    "nifDaCaessao": {
      "type": "string",
      "description": "Taxpayer Identification Number (NIF) of the assignee, if applicable."
    },
    "nomeDoCessionario": {
      "type": "string",
      "description": "Name of the assignee associated with the cessation of activity, if applicable."
    },
    "atividadeConstante": {
      "type": "string",
      "description": "Indicates whether the taxpayer is engaged in ongoing activity."
    },
    "descricao": {
      "type": "string",
      "description": "Description of the special VAT regime, if applicable."
    },
    "tipoOperacoes": {
      "type": "string",
      "description": "Type of operations conducted by the taxpayer."
    },
    "proRataDeducaoIva": {
      "type": "string",
      "description": "Pro-rata deduction of VAT applicable to the taxpayer."
    },
    "transacaoIntracomunitariasBens": {
      "type": "string",
      "description": "Indicates whether the taxpayer engages in intra-community transactions involving goods."
    },
    "opcaoRenuncia": {
      "type": "string",
      "description": "Option to waive VAT exemption on real estate operations."
    },
    "opcaoRegime": {
      "type": "string",
      "description": "Option for a specific VAT taxation regime."
    },
    "opcaoPeriodicidade": {
      "type": "string",
      "description": "Monthly option for VAT."
    },
    "prestacao": {
      "type": "string",
      "description": "Provision or acquisition of intra-community services."
    },
    "importacoes": {
      "type": "string",
      "description": "Imports."
    },
    "exportacoes": {
      "type": "string",
      "description": "Exports."
    },
    "aquisicoes": {
      "type": "string",
      "description": "Intra-community acquisitions conducted by the taxpayer."
    },
    "trasnmissoes": {
      "type": "string",
      "description": "Intra-community transmissions conducted by the taxpayer."
    },
    "reembolsoSituacao": {
      "type": "string",
      "description": "Current status of the taxpayer's monthly VAT refunds."
    },
    "reembolsoDataInicio": {
      "type": "string",
      "description": "Start date of the period related to the taxpayer's VAT refund."
    },
    "reembolsoDataFim": {
      "type": "string",
      "description": "End date of the period related to the taxpayer's VAT refund."
    },
    "ivaDataInicio": {
      "type": "string",
      "description": "Start date of the Cash Accounting VAT regime."
    },
    "ivaDataFim": {
      "type": "string",
      "description": "End date of the Cash Accounting VAT regime."
    },
    "ivaMotivo": {
      "type": "string",
      "description": "Reason for exclusion from the Cash Accounting VAT regime."
    },
    "importacoesDataInicio": {
      "type": "string",
      "description": "Start date for the period of import transactions under the VAT declaration payment option."
    },
    "importacoesDataFim": {
      "type": "string",
      "description": "End date for the period of import transactions under the VAT declaration payment option."
    },
    "importacoesMotivo": {
      "type": "string",
      "description": "Reason for canceling the VAT declaration payment option for imports."
    },
    "forfetarioDataInicio": {
      "type": "string",
      "description": "Start date of the simplified (forfait) VAT regime, if applicable."
    },
    "forfetarioDataFim": {
      "type": "string",
      "description": "End date of the simplified (forfait) VAT regime, if applicable."
    },
    "forfetarioMotivo": {
      "type": "string",
      "description": "Reason for applying or ending the simplified (forfait) VAT regime."
    }
  }
}

```