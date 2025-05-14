---
title: Responsabilidade Crédito Details
excerpt: This endpoint returns a document about the Responsabilidade Crédito.
api:
  file: bizapis.json
  operationId: responsabilidade-crédito-details
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
> 💻 [block:html]{"html":"<h3  style=\"text-align:center;\">DOWNLOAD PROJECT</h3>\n<ul>\n  <li><a href=\"https://we.tl/t-AzI2NwT01R\">Java</li>\n  <li><a href=\"https://we.tl/t-RBmDAZqlGs\">Python</li>\n  <li><a href=\"https://we.tl/t-wrclKxJCCa\">C#</li>\n</ul>\n<!--\n<a href=\"https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download\">\n  <button>Download project demo</button>\n</a> -->"}[/block]

[block:html]
{
  "html": "<a href=\"https://www.bizapis.com/wp-content/uploads/2024/08/servico_responsabilidade_credito.mp4.mp4\" target=\"_blank\">To watch the video click here"
}
[/block]


# JSON Schema API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "requestId" : {
      "type" : "string",
      "description" : "Identificador único do pedido"
    },
    "summary" : {
      "type" : "object",
      "description" : "Resumo da informação",
      "properties" : {
        "nif" : {
          "type" : "string",
          "description" : "Número de Identificação Fiscal (NIF)"
        },
        "name" : {
          "type" : "string",
          "description" : "Nome do titular"
        },
        "homeLoan" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado aos créditos à habitação",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "relatedLoan" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado aos créditos conexos",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "personalLoan" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado aos créditos pessoais",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "financialLeasing" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado à locação financeira",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "carLoanExcludingFinancialLeasing" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado aos créditos automóveis excluindo locação financeira",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "otherLoans" : {
          "type" : "object",
          "description" : "Mapa do resumo relacionado a outros créditos",
          "additionalProperties" : {
            "type" : "array",
            "items" : {
              "type" : "object",
              "properties" : {
                "type" : {
                  "type" : "string",
                  "description" : "Tipo de crédito"
                },
                "amount" : {
                  "type" : "number",
                  "description" : "Quantia do crédito"
                }
              }
            }
          }
        },
        "loanOverrun" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado à ultrapassagem de crédito",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "overdraftFacility" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado à facilidade de descoberto",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "creditCard" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado aos cartões de crédito",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "creditCardWithFreeFloat" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado aos cartões de crédito com período de free float",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "creditCardWithoutFreeFloat" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado aos cartões de crédito sem período de free float",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "deferredDebitCard" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado aos cartões de débito diferido",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "revolvingCredit" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado aos créditos renováveis",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "nonRevolvingCredit" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado aos créditos não renováveis",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              }
            }
          }
        },
        "outstandingAmount" : {
          "type" : "array",
          "description" : "Lista do resumo relacionado aos montantes em dívida",
          "items" : {
            "type" : "object",
            "properties" : {
              "type" : {
                "type" : "string",
                "description" : "Tipo de crédito"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia do crédito"
              },
              "isOutstandingAmountFromCreditCard" : {
                "type" : "boolean",
                "description" : "Indica se o montante em dívida é proveniente de um cartão de crédito"
              }
            }
          }
        }
      }
    },
    "homeLoan" : {
      "type" : "array",
      "description" : "Lista de créditos à habitação",
      "items" : {
        "type" : "object",
        "properties" : {
          "startDate" : {
            "type" : "string",
            "description" : "Data de início do crédito"
          },
          "endDate" : {
            "type" : "string",
            "description" : "Data de fim do crédito"
          },
          "numberDebtors" : {
            "type" : "integer",
            "description" : "Número de devedores no contrato"
          },
          "totalDebt" : {
            "type" : "number",
            "description" : "Total da dívida"
          },
          "installment" : {
            "type" : "number",
            "description" : "Valor da prestação"
          }
        }
      }
    },
    "carLoan" : {
      "type" : "array",
      "description" : "Lista de créditos automóveis",
      "items" : {
        "type" : "object",
        "properties" : {
          "startDate" : {
            "type" : "string",
            "description" : "Data de início do crédito"
          },
          "endDate" : {
            "type" : "string",
            "description" : "Data de fim do crédito"
          },
          "numberDebtors" : {
            "type" : "integer",
            "description" : "Número de devedores no contrato"
          },
          "totalDebt" : {
            "type" : "number",
            "description" : "Total da dívida"
          },
          "installment" : {
            "type" : "number",
            "description" : "Valor da prestação"
          }
        }
      }
    },
    "financialLeasing" : {
      "type" : "array",
      "description" : "Lista de Locações Financeiras",
      "items" : {
        "type" : "object",
        "properties" : {
          "startDate" : {
            "type" : "string",
            "description" : "Data de início do crédito"
          },
          "endDate" : {
            "type" : "string",
            "description" : "Data de fim do crédito"
          },
          "numberDebtors" : {
            "type" : "integer",
            "description" : "Número de devedores no contrato"
          },
          "totalDebt" : {
            "type" : "number",
            "description" : "Total da dívida"
          },
          "installment" : {
            "type" : "number",
            "description" : "Valor da prestação"
          }
        }
      }
    },
    "otherLoans" : {
      "type" : "object",
      "description" : "Lista de outros créditos",
      "additionalProperties" : {
        "type" : "array",
        "items" : {
          "type" : "object",
          "properties" : {
            "startDate" : {
              "type" : "string",
              "description" : "Data de início do crédito"
            },
            "endDate" : {
              "type" : "string",
              "description" : "Data de fim do crédito"
            },
            "numberDebtors" : {
              "type" : "integer",
              "description" : "Número de devedores no contrato"
            },
            "totalDebt" : {
              "type" : "number",
              "description" : "Total da dívida"
            },
            "installment" : {
              "type" : "number",
              "description" : "Valor da prestação"
            }
          }
        }
      }
    },
    "personalLoan" : {
      "type" : "array",
      "description" : "Lista de créditos pessoais",
      "items" : {
        "type" : "object",
        "properties" : {
          "startDate" : {
            "type" : "string",
            "description" : "Data de início do crédito"
          },
          "endDate" : {
            "type" : "string",
            "description" : "Data de fim do crédito"
          },
          "numberDebtors" : {
            "type" : "integer",
            "description" : "Número de devedores no contrato"
          },
          "totalDebt" : {
            "type" : "number",
            "description" : "Total da dívida"
          },
          "installment" : {
            "type" : "number",
            "description" : "Valor da prestação"
          }
        }
      }
    },
    "relatedLoan" : {
      "type" : "array",
      "description" : "Lista de créditos conexos",
      "items" : {
        "type" : "object",
        "properties" : {
          "startDate" : {
            "type" : "string",
            "description" : "Data de início do crédito"
          },
          "endDate" : {
            "type" : "string",
            "description" : "Data de fim do crédito"
          },
          "numberDebtors" : {
            "type" : "integer",
            "description" : "Número de devedores no contrato"
          },
          "totalDebt" : {
            "type" : "number",
            "description" : "Total da dívida"
          },
          "installment" : {
            "type" : "number",
            "description" : "Valor da prestação"
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
    "requestId": {
      "type": "string",
      "description": "A unique identifier for the request."
    },
    "summary": {
      "type": "object",
      "description": "A summarized view of the credit information.",
      "properties": {
        "nif": {
          "type": "string",
          "description": "Tax Identification Number (NIF)."
        },
        "name": {
          "type": "string",
          "description": "Name of the account holder."
        },
        "homeLoan": {
          "type": "array",
          "description": "A list summarizing home loans.",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit."
              },
              "amount": {
                "type": "number",
                "description": "Loan amount."
              }
            }
          }
        },
        "relatedLoan": {
          "type": "array",
          "description": "A list summarizing related loans.",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit."
              },
              "amount": {
                "type": "number",
                "description": "Loan amount."
              }
            }
          }
        },
        "personalLoan": {
          "type": "array",
          "description": "A list summarizing personal loans.",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit."
              },
              "amount": {
                "type": "number",
                "description": "Loan amount."
              }
            }
          }
        },
        "financialLeasing": {
          "type": "array",
          "description": "A summary of financial leasing agreements.",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit."
              },
              "amount": {
                "type": "number",
                "description": "Loan amount."
              }
            }
          }
        },
        "carLoanExcludingFinancialLeasing": {
          "type": "array",
          "description": "A list of car loans, excluding financial leasing.",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit."
              },
              "amount": {
                "type": "number",
                "description": "Loan amount."
              }
            }
          }
        },
        "otherLoans": {
          "type": "object",
          "description": "A map summarizing other types of loans.",
          "additionalProperties": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "type": {
                  "type": "string",
                  "description": "Type of credit."
                },
                "amount": {
                  "type": "number",
                  "description": "Loan amount."
                }
              }
            }
          }
        },
        "loanOverrun": {
          "type": "array",
          "description": "A list summarizing loan overruns.",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit."
              },
              "amount": {
                "type": "number",
                "description": "Loan amount."
              }
            }
          }
        },
        "overdraftFacility": {
          "type": "array",
          "description": "A summary of overdraft facilities.",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit."
              },
              "amount": {
                "type": "number",
                "description": "Loan amount."
              }
            }
          }
        },
        "creditCard": {
          "type": "array",
          "description": "A list summarizing credit card obligations.",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit."
              },
              "amount": {
                "type": "number",
                "description": "Loan amount."
              }
            }
          }
        },
        "outstandingAmount": {
          "type": "array",
          "description": "A summary of outstanding debt.",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit."
              },
              "amount": {
                "type": "number",
                "description": "Outstanding amount."
              },
              "isOutstandingAmountFromCreditCard": {
                "type": "boolean",
                "description": "Indicates whether the outstanding amount originates from a credit card."
              }
            }
          }
        }
      }
    },
    "homeLoan": {
      "type": "array",
      "description": "A detailed list of home loans.",
      "items": {
        "type": "object",
        "properties": {
          "startDate": {
            "type": "string",
            "description": "Loan start date."
          },
          "endDate": {
            "type": "string",
            "description": "Loan end date."
          },
          "numberDebtors": {
            "type": "integer",
            "description": "Number of debtors in the contract."
          },
          "totalDebt": {
            "type": "number",
            "description": "Total outstanding debt."
          },
          "installment": {
            "type": "number",
            "description": "Monthly installment amount."
          }
        }
      }
    },
    "carLoan": {
      "type": "array",
      "description": "A detailed list of car loans.",
      "items": {
        "type": "object",
        "properties": {
          "startDate": {
            "type": "string",
            "description": "Loan start date."
          },
          "endDate": {
            "type": "string",
            "description": "Loan end date."
          },
          "numberDebtors": {
            "type": "integer",
            "description": "Number of debtors in the contract."
          },
          "totalDebt": {
            "type": "number",
            "description": "Total outstanding debt."
          },
          "installment": {
            "type": "number",
            "description": "Monthly installment amount."
          }
        }
      }
    },
    "financialLeasing": {
      "type": "array",
      "description": "Details of financial leasing agreements.",
      "items": {
        "type": "object",
        "properties": {
          "startDate": {
            "type": "string",
            "description": "Loan start date."
          },
          "endDate": {
            "type": "string",
            "description": "Loan end date."
          },
          "numberDebtors": {
            "type": "integer",
            "description": "Number of debtors in the contract."
          },
          "totalDebt": {
            "type": "number",
            "description": "Total outstanding debt."
          },
          "installment": {
            "type": "number",
            "description": "Monthly installment amount."
          }
        }
      }
    },
    "personalLoan": {
      "type": "array",
      "description": "A list of personal loans.",
      "items": {
        "type": "object",
        "properties": {
          "startDate": {
            "type": "string",
            "description": "Loan start date."
          },
          "endDate": {
            "type": "string",
            "description": "Loan end date."
          },
          "numberDebtors": {
            "type": "integer",
            "description": "Number of debtors in the contract."
          },
          "totalDebt": {
            "type": "number",
            "description": "Total outstanding debt."
          },
          "installment": {
            "type": "number",
            "description": "Monthly installment amount."
          }
        }
      }
    }
  }
}

```