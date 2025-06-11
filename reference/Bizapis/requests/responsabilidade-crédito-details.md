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
```Text ENG
```

## English (ENG)

```json
{
  "type": "object",
  "properties": {
    "data": {
      "type": "object",
      "properties": {
        "requestId": {
          "type": "string",
          "description": "Unique request identifier"
        }
      }
    },
    "file": {
      "type": "string",
      "description": "Encoded base 64 file."
    }
  }
}
```