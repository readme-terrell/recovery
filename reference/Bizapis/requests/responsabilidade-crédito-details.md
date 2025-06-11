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
# Download Project

* [Java](https://we.tl/t-AzI2NwT01R)
* [Python](https://we.tl/t-RBmDAZqlGs)
* [C#](https://we.tl/t-wrclKxJCCa)

[Watch the video](https://www.bizapis.com/wp-content/uploads/2024/08/servico_responsabilidade_credito.mp4.mp4)

# JSON Schema API Response

## Portuguese (PT)

```json JSON
{
  "type" : "object",
  "properties" : {
    "requestId" : {
      "type" : "string",
      "description" : "Identificador único do pedido"
    },
    "summary" : {
      "type" : "object",
      "description" : "Resumo das Responsabilidades de Crédito",
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                  "description" : "Tipo de crédito (pode ser conjunto ou individual)"
                },
                "amount" : {
                  "type" : "number",
                  "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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
                "description" : "Tipo de crédito (pode ser conjunto ou individual)"
              },
              "amount" : {
                "type" : "number",
                "description" : "Quantia total do crédito"
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

## English (ENG)

```json
{
  "type": "object",
  "properties": {
    "requestId": {
      "type": "string",
      "description": "Unique identifier of the request"
    },
    "summary": {
      "type": "object",
      "description": "Credit Responsibilities Summary",
      "properties": {
        "nif": {
          "type": "string",
          "description": "Tax Identification Number (TIN)"
        },
        "name": {
          "type": "string",
          "description": "Name of the holder"
        },
        "homeLoan": {
          "type": "array",
          "description": "Summary list related to home loans",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "relatedLoan": {
          "type": "array",
          "description": "Summary list related to related loans",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "personalLoan": {
          "type": "array",
          "description": "Summary list related to personal loans",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "financialLeasing": {
          "type": "array",
          "description": "Summary list related to financial leasing",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "carLoanExcludingFinancialLeasing": {
          "type": "array",
          "description": "Summary list related to car loans excluding financial leasing",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "otherLoans": {
          "type": "object",
          "description": "Map of the summary related to other credits",
          "additionalProperties": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "type": {
                  "type": "string",
                  "description": "Type of credit (can be joint or individual)"
                },
                "amount": {
                  "type": "number",
                  "description": "Total credit amount"
                }
              }
            }
          }
        },
        "loanOverrun": {
          "type": "array",
          "description": "Summary list related to credit overrun",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "overdraftFacility": {
          "type": "array",
          "description": "Summary list related to overdraft facility",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "creditCard": {
          "type": "array",
          "description": "Summary list related to credit cards",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "creditCardWithFreeFloat": {
          "type": "array",
          "description": "Summary list related to credit cards with free float period",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "creditCardWithoutFreeFloat": {
          "type": "array",
          "description": "Summary list related to credit cards without free float period",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "deferredDebitCard": {
          "type": "array",
          "description": "Summary list related to deferred debit cards",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "revolvingCredit": {
          "type": "array",
          "description": "Summary list related to revolving credits",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "nonRevolvingCredit": {
          "type": "array",
          "description": "Summary list related to non-revolving credits",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              }
            }
          }
        },
        "outstandingAmount": {
          "type": "array",
          "description": "Summary list related to outstanding amounts",
          "items": {
            "type": "object",
            "properties": {
              "type": {
                "type": "string",
                "description": "Type of credit (can be joint or individual)"
              },
              "amount": {
                "type": "number",
                "description": "Total credit amount"
              },
              "isOutstandingAmountFromCreditCard": {
                "type": "boolean",
                "description": "Indicates whether the outstanding amount is from a credit card"
              }
            }
          }
        }
      }
    },
    "homeLoan": {
      "type": "array",
      "description": "List of home loans",
      "items": {
        "type": "object",
        "properties": {
          "startDate": {
            "type": "string",
            "description": "Start date of the loan"
          },
          "endDate": {
            "type": "string",
            "description": "End date of the loan"
          },
          "numberDebtors": {
            "type": "integer",
            "description": "Number of debtors in the contract"
          },
          "totalDebt": {
            "type": "number",
            "description": "Total debt"
          },
          "installment": {
            "type": "number",
            "description": "Installment amount"
          }
        }
      }
    },
    "carLoan": {
      "type": "array",
      "description": "List of car loans",
      "items": {
        "type": "object",
        "properties": {
          "startDate": {
            "type": "string",
            "description": "Start date of the loan"
          },
          "endDate": {
            "type": "string",
            "description": "End date of the loan"
          },
          "numberDebtors": {
            "type": "integer",
            "description": "Number of debtors in the contract"
          },
          "totalDebt": {
            "type": "number",
            "description": "Total debt"
          },
          "installment": {
            "type": "number",
            "description": "Installment amount"
          }
        }
      }
    },
    "financialLeasing": {
      "type": "array",
      "description": "List of financial leasing contracts",
      "items": {
        "type": "object",
        "properties": {
          "startDate": {
            "type": "string",
            "description": "Start date of the loan"
          },
          "endDate": {
            "type": "string",
            "description": "End date of the loan"
          },
          "numberDebtors": {
            "type": "integer",
            "description": "Number of debtors in the contract"
          },
          "totalDebt": {
            "type": "number",
            "description": "Total debt"
          },
          "installment": {
            "type": "number",
            "description": "Installment amount"
          }
        }
      }
    },
    "otherLoans": {
      "type": "object",
      "description": "List of other loans",
      "additionalProperties": {
        "type": "array",
        "items": {
          "type": "object",
          "properties": {
            "startDate": {
              "type": "string",
              "description": "Start date of the loan"
            },
            "endDate": {
              "type": "string",
              "description": "End date of the loan"
            },
            "numberDebtors": {
              "type": "integer",
              "description": "Number of debtors in the contract"
            },
            "totalDebt": {
              "type": "number",
              "description": "Total debt"
            },
            "installment": {
              "type": "number",
              "description": "Installment amount"
            }
          }
        }
      }
    },
    "personalLoan": {
      "type": "array",
      "description": "List of personal loans",
      "items": {
        "type": "object",
        "properties": {
          "startDate": {
            "type": "string",
            "description": "Start date of the loan"
          },
          "endDate": {
            "type": "string",
            "description": "End date of the loan"
          },
          "numberDebtors": {
            "type": "integer",
            "description": "Number of debtors in the contract"
          },
          "totalDebt": {
            "type": "number",
            "description": "Total debt"
          },
          "installment": {
            "type": "number",
            "description": "Installment amount"
          }
        }
      }
    },
    "relatedLoan": {
      "type": "array",
      "description": "List of related loans",
      "items": {
        "type": "object",
        "properties": {
          "startDate": {
            "type": "string",
            "description": "Start date of the loan"
          },
          "endDate": {
            "type": "string",
            "description": "End date of the loan"
          },
          "numberDebtors": {
            "type": "integer",
            "description": "Number of debtors in the contract"
          },
          "totalDebt": {
            "type": "number",
            "description": "Total debt"
          },
          "installment": {
            "type": "number",
            "description": "Installment amount"
          }
        }
      }
    }
  }
}

```