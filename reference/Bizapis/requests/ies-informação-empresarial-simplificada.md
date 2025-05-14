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
> 💻 [block:html]{"html":"<h3  style=\"text-align:center;\">DOWNLOAD PROJECT</h3>\n<ul>\n  <li><a href=\"https://we.tl/t-8U051WQwfe\">Java</li>\n  <li><a href=\"https://we.tl/t-ynSKuElrpE\">Python</li>\n  <li><a href=\"https://we.tl/t-4SaCPBTr7A\">C#</li>\n</ul>\n<!--\n<a href=\"https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download\">\n  <button>Download project demo</button>\n</a> -->"}[/block]

[block:html]
{
  "html": "<a href=\"https://www.bizapis.com/wp-content/uploads/2024/08/seervico_informacao_empresarial_simplificada.mp4.mp4\" target=\"_blank\">To watch the video click here"
}
[/block]


# JSON Schema API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "anexoA" : {
      "type" : "object",
      "description" : "Anexo A",
      "properties" : {
        "q0101_nif" : {
          "type" : "integer",
          "description" : "Número de identificação fiscal (NIF) da empresa"
        },
        "q0102_exercicio" : {
          "type" : "string",
          "description" : "Ano de pesquisa"
        },
        "q03_A5001" : {
          "type" : "number",
          "description" : "Vendas e serviços prestados"
        },
        "q03_A5002" : {
          "type" : "number",
          "description" : "Subsídios à exploração"
        },
        "q03_A5003" : {
          "type" : "number",
          "description" : "Ganhos/perdas imputadas de subsidiárias e empreendimentos conjuntos"
        },
        "q03_A5004" : {
          "type" : "number",
          "description" : "Variação nos inventários da produção"
        },
        "q03_A5005" : {
          "type" : "number",
          "description" : "Trabalhos para a própria entidade"
        },
        "q03_A5006" : {
          "type" : "number",
          "description" : "Custos das mercadorias vendidas e das matérias consumidas"
        },
        "q03_A5007" : {
          "type" : "number",
          "description" : "Fornecimentos e serviços externos"
        },
        "q03_A5008" : {
          "type" : "number",
          "description" : "Gastos com o pessoal"
        },
        "q03_A5009" : {
          "type" : "number",
          "description" : "Imparidade de inventários (perdas/reversões)"
        },
        "q03_A5010" : {
          "type" : "number",
          "description" : "Imparidade de dívidas a receber (perdas/reversões)"
        },
        "q03_A5011" : {
          "type" : "number",
          "description" : "Provisões (aumentos/reduções)"
        },
        "q03_A5012" : {
          "type" : "number",
          "description" : "Imparidade de investimentos não depreciáveis/amortizáveis (perdas/reversões)"
        },
        "q03_A5013" : {
          "type" : "number",
          "description" : "Outras imparidades (perdas/reversões) / Imparidades (perdas/reversões) (utilização exclusiva pelas pequenas entidades e microentidades)"
        },
        "q03_A5014" : {
          "type" : "number",
          "description" : "Aumentos/reduções de justo valor"
        },
        "q03_A5015" : {
          "type" : "number",
          "description" : "Outros rendimentos e ganhos"
        },
        "q03_A5016" : {
          "type" : "number",
          "description" : "Outros gastos e perdas"
        },
        "q03_A5017" : {
          "type" : "number",
          "description" : "Resultado antes de depreciações, gastos de financiamento e impostos"
        },
        "q03_A5018" : {
          "type" : "number",
          "description" : "Gastos/reversões de depreciação e de amortização"
        },
        "q03_A5019" : {
          "type" : "number",
          "description" : "Imparidade de investimentos depreciáveis/amortizáveis (perdas/reversões)"
        },
        "q03_A5020" : {
          "type" : "number",
          "description" : "Resultado operacional (antes de gastos de financiamento e impostos)"
        },
        "q03_A5021" : {
          "type" : "number",
          "description" : "Juros e rendimentos similares obtidos"
        },
        "q03_A5022" : {
          "type" : "number",
          "description" : "Juros e gastos similares suportados"
        },
        "q03_A5023" : {
          "type" : "number",
          "description" : "Resultado antes de impostos"
        },
        "q03_A5024" : {
          "type" : "number",
          "description" : "Imposto sobre o rendimento do período"
        },
        "q03_A5025" : {
          "type" : "number",
          "description" : "Resultado líquido do período"
        },
        "q03_A5026" : {
          "type" : "number",
          "description" : "Resultado das atividades descontinuadas (líquido de impostos) incluído no resultado líquido do período"
        },
        "q04_A5101" : {
          "type" : "number",
          "description" : "Ativos fixos tangíveis"
        },
        "q04_A5102" : {
          "type" : "number",
          "description" : "Propriedades de investimento"
        },
        "q04_A5103" : {
          "type" : "number",
          "description" : "Goodwill"
        },
        "q04_A5104" : {
          "type" : "number",
          "description" : "Ativos intangíveis"
        },
        "q04_A5105" : {
          "type" : "number",
          "description" : "Ativos biológicos"
        },
        "q04_A5106" : {
          "type" : "number",
          "description" : "Participações financeiras - método da equivalência patrimonial"
        },
        "q04_A5107" : {
          "type" : "number",
          "description" : "Participações financeiras - outros métodos"
        },
        "q04_A5108" : {
          "type" : "number",
          "description" : "Accionistas / sócios"
        },
        "q04_A5109" : {
          "type" : "number",
          "description" : "Outros ativos financeiros"
        },
        "q04_A5110" : {
          "type" : "number",
          "description" : "Activos por impostos diferidos"
        },
        "q04_A5111" : {
          "type" : "number",
          "description" : "Investimentos financeiros (utilização exclusiva pelas pequenas entidades e microentidades)"
        },
        "q04_A5112" : {
          "type" : "number",
          "description" : "SOMA"
        },
        "q04_A5113" : {
          "type" : "number",
          "description" : "Inventários"
        },
        "q04_A5114" : {
          "type" : "number",
          "description" : "Activos biológicos"
        },
        "q04_A5115" : {
          "type" : "number",
          "description" : "Clientes"
        },
        "q04_A5116" : {
          "type" : "number",
          "description" : "Adiantamentos a fornecedores"
        },
        "q04_A5117" : {
          "type" : "number",
          "description" : "Estado e outros entes públicos"
        },
        "q04_A5118" : {
          "type" : "number",
          "description" : "Accionistas / sócios"
        },
        "q04_A5119" : {
          "type" : "number",
          "description" : "Outras contas a receber"
        },
        "q04_A5120" : {
          "type" : "number",
          "description" : "Diferimentos"
        },
        "q04_A5121" : {
          "type" : "number",
          "description" : "Activos financeiros detidos para negociação"
        },
        "q04_A5122" : {
          "type" : "number",
          "description" : "Outros activos financeiros"
        },
        "q04_A5123" : {
          "type" : "number",
          "description" : "Activos não correntes detidos para venda"
        },
        "q04_A5124" : {
          "type" : "number",
          "description" : "Outros activos correntes"
        },
        "q04_A5125" : {
          "type" : "number",
          "description" : "Caixa e depósitos bancários"
        },
        "q04_A5126" : {
          "type" : "number",
          "description" : "SOMA"
        },
        "q04_A5127" : {
          "type" : "number",
          "description" : "TOTAL DO ACTIVO"
        },
        "q04_A5128" : {
          "type" : "number",
          "description" : "Capital realizado"
        },
        "q04_A5129" : {
          "type" : "number",
          "description" : "Acções (quotas) próprias"
        },
        "q04_A5130" : {
          "type" : "number",
          "description" : "Outros instrumentos de capital próprio"
        },
        "q04_A5131" : {
          "type" : "number",
          "description" : "Prémios de emissão"
        },
        "q04_A5132" : {
          "type" : "number",
          "description" : "Reservas legais"
        },
        "q04_A5133" : {
          "type" : "number",
          "description" : "Outras reservas"
        },
        "q04_A5134" : {
          "type" : "number",
          "description" : "Resultados transitados"
        },
        "q04_A5135" : {
          "type" : "number",
          "description" : "Ajustamnetos em activos financeiros"
        },
        "q04_A5136" : {
          "type" : "number",
          "description" : "Excendentes de revalorização"
        },
        "q04_A5137" : {
          "type" : "number",
          "description" : "Outras variações no capital próprio"
        },
        "q04_A5138" : {
          "type" : "number",
          "description" : "SOMA"
        },
        "q04_A5139" : {
          "type" : "number",
          "description" : "Resultado líquido do período"
        },
        "q04_A5140" : {
          "type" : "number",
          "description" : "Dividendos antecipados"
        },
        "q04_A5141" : {
          "type" : "number",
          "description" : "Total do capital próprio"
        },
        "q04_A5142" : {
          "type" : "number",
          "description" : "Provisões"
        },
        "q04_A5143" : {
          "type" : "number",
          "description" : "Financiamentos obtidos"
        },
        "q04_A5144" : {
          "type" : "number",
          "description" : "Responsabilidades por benefícios pós-emprego"
        },
        "q04_A5145" : {
          "type" : "number",
          "description" : "Passivos por impostos diferidos"
        },
        "q04_A5146" : {
          "type" : "number",
          "description" : "Outras contas a pagar"
        },
        "q04_A5147" : {
          "type" : "number",
          "description" : "SOMA"
        },
        "q04_A5148" : {
          "type" : "number",
          "description" : "Fornecedores"
        },
        "q04_A5149" : {
          "type" : "number",
          "description" : "Adiantamentos de clientes"
        },
        "q04_A5150" : {
          "type" : "number",
          "description" : "Estado e outros entes públicos"
        },
        "q04_A5151" : {
          "type" : "number",
          "description" : "Accisonistas / sócios"
        },
        "q04_A5152" : {
          "type" : "number",
          "description" : "Financiamentos obtidos"
        },
        "q04_A5153" : {
          "type" : "number",
          "description" : "Outras contas a pagar"
        },
        "q04_A5154" : {
          "type" : "number",
          "description" : "Diferimentos"
        },
        "q04_A5155" : {
          "type" : "number",
          "description" : "Passivos financeiros detidos para negociação"
        },
        "q04_A5156" : {
          "type" : "number",
          "description" : "Outros passivos financeiros"
        },
        "q04_A5157" : {
          "type" : "number",
          "description" : "Passivos não correntes detidos para venda"
        },
        "q04_A5158" : {
          "type" : "number",
          "description" : "Outros passivos correntes"
        },
        "q04_A5159" : {
          "type" : "number",
          "description" : "SOMA"
        },
        "q04_A5160" : {
          "type" : "number",
          "description" : "TOTAL DO PASSIVO"
        },
        "q04_A5161" : {
          "type" : "number",
          "description" : "TOTAL DO PASSIVO E CAPITAL PRÓPRIO"
        },
        "q05291_A6012" : {
          "type" : "integer",
          "description" : "Pessoas ao serviço da empresa, remuneradas e não remuneradas"
        },
        "q05291_A6013" : {
          "type" : "integer",
          "description" : "Pessoas remuneradas ao serviço da empresa"
        },
        "q05291_A6014" : {
          "type" : "integer",
          "description" : "Pessoas não remuneradas ao serviço da empresa"
        },
        "q05291_A6015" : {
          "type" : "integer",
          "description" : "Pessoas ao serviço da empresa a tempo completo"
        },
        "q05291_A6016" : {
          "type" : "integer",
          "description" : "Das quais: Pessoas remuneradas ao serviço da empresa a tempo completo"
        },
        "q05291_A6017" : {
          "type" : "integer",
          "description" : "Pessoas ao serviço da empresa a tempo parcial"
        },
        "q05291_A6018" : {
          "type" : "integer",
          "description" : "Das quais: Pessoas remuneradas ao serviço da empresa a tempo parcial"
        },
        "q05291_A6019" : {
          "type" : "integer",
          "description" : "Pessoas ao serviço da empresa, por sexo: Homens"
        },
        "q05291_A6020" : {
          "type" : "integer",
          "description" : "Pessoas ao serviço da empresa, por sexo: Mulheres"
        },
        "q05291_A6021" : {
          "type" : "integer",
          "description" : "Pessoas ao serviço da empresa, afectas à Investigação e Desenvolvimento"
        },
        "q05291_A6022" : {
          "type" : "integer",
          "description" : "Prestadores de serviços"
        },
        "q05291_A6023" : {
          "type" : "integer",
          "description" : "Pessoas colocadas através de agências de trabalho temporário"
        }
      }
    },
    "rosto" : {
      "type" : "object",
      "properties" : {
        "q01Ano" : {
          "type" : "integer",
          "description" : "Ano de pesquisa"
        },
        "q03Name" : {
          "type" : "string",
          "description" : "Nome da empresa"
        },
        "q03Nif" : {
          "type" : "integer",
          "description" : "Número de identificação fiscal (NIF) da empresa"
        }
      }
    },
    "requestId" : {
      "type" : "string",
      "description" : "Identificador único do pedido"
    }
  }
}
```
```json ENG
{
  "type": "object",
  "properties": {
    "anexoA": {
      "type": "object",
      "description": "Annex A",
      "properties": {
        "q0101_nif": {
          "type": "integer",
          "description": "Tax Identification Number (NIF)"
        },
        "q0102_exercicio": {
          "type": "string",
          "description": "Fiscal Year"
        },
        "q03_A5001": {
          "type": "number",
          "description": "Revenue from Sales and Services Rendered"
        },
        "q03_A5002": {
          "type": "number",
          "description": "Operating Subsidies"
        },
        "q03_A5003": {
          "type": "number",
          "description": "Gains/Losses Attributable to Subsidiaries and Joint Ventures"
        },
        "q03_A5004": {
          "type": "number",
          "description": "Changes in Inventory of Finished Goods and Work in Progress"
        },
        "q03_A5005": {
          "type": "number",
          "description": "Work Performed for the Entity Itself"
        },
        "q03_A5006": {
          "type": "number",
          "description": "Cost of Goods Sold and Raw Materials Consumed"
        },
        "q03_A5007": {
          "type": "number",
          "description": "Supplies and External Services"
        },
        "q03_A5008": {
          "type": "number",
          "description": "Employee Expenses"
        },
        "q03_A5009": {
          "type": "number",
          "description": "Impairment of Inventories (Losses/Reversals)"
        },
        "q03_A5010": {
          "type": "number",
          "description": "Impairment of Receivables (Losses/Reversals)"
        },
        "q03_A5011": {
          "type": "number",
          "description": "Provisions (Increases/Decreases)"
        },
        "q03_A5012": {
          "type": "number",
          "description": "Impairment of Non-Depreciable/Amortizable Investments (Losses/Reversals)"
        },
        "q03_A5013": {
          "type": "number",
          "description": "Other Impairments (Losses/Reversals) (Exclusive Use by Small and Micro Entities)"
        },
        "q03_A5014": {
          "type": "number",
          "description": "Fair Value Adjustments (Increases/Decreases)"
        },
        "q03_A5015": {
          "type": "number",
          "description": "Other Income and Gains"
        },
        "q03_A5016": {
          "type": "number",
          "description": "Other Expenses and Losses"
        },
        "q03_A5017": {
          "type": "number",
          "description": "Earnings Before Depreciation, Financial Expenses, and Taxes"
        },
        "q03_A5018": {
          "type": "number",
          "description": "Depreciation and Amortization Expenses/Reversals"
        },
        "q03_A5019": {
          "type": "number",
          "description": "Impairment of Depreciable/Amortizable Investments (Losses/Reversals)"
        },
        "q03_A5020": {
          "type": "number",
          "description": "Operating Profit (Before Financial Expenses and Taxes)"
        },
        "q03_A5021": {
          "type": "number",
          "description": "Interest and Similar Income"
        },
        "q03_A5022": {
          "type": "number",
          "description": "Interest and Similar Expenses"
        },
        "q03_A5023": {
          "type": "number",
          "description": "Profit Before Taxes"
        },
        "q03_A5024": {
          "type": "number",
          "description": "Income Tax for the Period"
        },
        "q03_A5025": {
          "type": "number",
          "description": "Net Profit for the Period"
        },
        "q03_A5026": {
          "type": "number",
          "description": "Profit from Discontinued Operations (Net of Taxes) Included in Net Profit for the Period"
        },
        "q04_A5101": {
          "type": "number",
          "description": "Tangible Fixed Assets"
        },
        "q04_A5102": {
          "type": "number",
          "description": "Investment Properties"
        },
        "q04_A5103": {
          "type": "number",
          "description": "Goodwill"
        },
        "q04_A5104": {
          "type": "number",
          "description": "Intangible Assets"
        },
        "q04_A5105": {
          "type": "number",
          "description": "Biological Assets"
        },
        "q04_A5106": {
          "type": "number",
          "description": "Financial Investments - Equity Method"
        },
        "q04_A5107": {
          "type": "number",
          "description": "Financial Investments - Other Methods"
        },
        "q04_A5108": {
          "type": "number",
          "description": "Shareholders/Partners"
        },
        "q04_A5109": {
          "type": "number",
          "description": "Other Financial Assets"
        },
        "q04_A5110": {
          "type": "number",
          "description": "Deferred Tax Assets"
        },
        "q04_A5111": {
          "type": "number",
          "description": "Financial Investments (Exclusive Use by Small and Micro Entities)"
        },
        "q04_A5112": {
          "type": "number",
          "description": "TOTAL"
        },
        "q05291_A6012": {
          "type": "integer",
          "description": "Total Employees, Including Paid and Unpaid"
        },
        "q05291_A6013": {
          "type": "integer",
          "description": "Total Paid Employees"
        },
        "q05291_A6014": {
          "type": "integer",
          "description": "Total Unpaid Employees"
        },
        "q05291_A6015": {
          "type": "integer",
          "description": "Full-Time Employees"
        },
        "q05291_A6016": {
          "type": "integer",
          "description": "Of Which: Paid Full-Time Employees"
        },
        "q05291_A6017": {
          "type": "integer",
          "description": "Part-Time Employees"
        },
        "q05291_A6018": {
          "type": "integer",
          "description": "Of Which: Paid Part-Time Employees"
        },
        "q05291_A6019": {
          "type": "integer",
          "description": "Total Male Employees"
        },
        "q05291_A6020": {
          "type": "integer",
          "description": "Total Female Employees"
        },
        "q05291_A6021": {
          "type": "integer",
          "description": "Employees Assigned to Research and Development"
        },
        "q05291_A6022": {
          "type": "integer",
          "description": "Service Providers"
        },
        "q05291_A6023": {
          "type": "integer",
          "description": "Employees Hired Through Temporary Employment Agencies"
        }
      }
    },
    "rosto": {
      "type": "object",
      "properties": {
        "q01Ano": {
          "type": "integer",
          "description": "Research Year"
        },
        "q03Name": {
          "type": "string",
          "description": "Company Name"
        },
        "q03Nif": {
          "type": "integer",
          "description": "Company Tax Identification Number (NIF)"
        }
      }
    },
    "requestId": {
      "type": "string",
      "description": "Unique Request Identifier"
    }
  }
}

```