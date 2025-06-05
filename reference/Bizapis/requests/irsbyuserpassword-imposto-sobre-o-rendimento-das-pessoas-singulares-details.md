---
title: IRSByUserPassword Details (Imposto sobre o Rendimento das Pessoas Singulares)
excerpt: Endpoint to retrieve information from the IRS Mod3 document.
api:
  file: bizapis.json
  operationId: irsbyuserpassword-imposto-sobre-o-rendimento-das-pessoas-singulares-details
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

* [Java](https://we.tl/t-i2uXcW3RSJ)
* [Python](https://we.tl/t-6aDYiqD1G2)
* [C#](https://we.tl/t-TaJQ6xfayh)

# JSON Schema for API Response

```json ENG
{
  "type" : "object",
  "properties" : {
    "requestId" : {
      "type" : "string",
      "description" : "Unique identifier for the request."
    },
    "intro" : {
      "type" : "object",
      "description" : "Introductory information section of the declaration.",
      "properties" : {
        "yearOfIncome" : {
          "type" : "string",
          "description" : "Year to which the declared income relates."
        },
        "taxpayerNIFA" : {
          "type" : "string",
          "description" : "Taxpayer NIF (Número de Identificação Fiscal) for taxpayer A."
        },
        "taxpayerNIFB" : {
          "type" : "string",
          "description" : "Taxpayer NIF (Número de Identificação Fiscal) for taxpayer B."
        }
      }
    },
    "catA" : {
      "type" : "object",
      "description" : "Category A — Income from dependent work.",
      "properties" : {
        "incomeFromDependentWorkSum" : {
          "type" : "number",
          "description" : "Sum of income from dependent work."
        },
        "withholdingTaxSum" : {
          "type" : "number",
          "description" : "Sum of withholding tax applied to dependent work income."
        },
        "contributionsSum" : {
          "type" : "number",
          "description" : "Sum of social security contributions deducted from dependent work income."
        },
        "surtaxWithholdingSum" : {
          "type" : "number",
          "description" : "Sum of surtax withholding applied to dependent work income."
        },
        "unionDuesSum" : {
          "type" : "number",
          "description" : "Sum of union dues deducted from dependent work income."
        }
      }
    },
    "catB" : {
      "type" : "object",
      "description" : "Category B — Income from business and professional activities.",
      "properties" : {
        "grossProfessionalCommercialAndIndustrialIncomeSum" : {
          "type" : "number",
          "description" : "Sum of gross income from professional, commercial, and industrial activities."
        },
        "grossAgriculturalForestryAndLivestockIncomeSum" : {
          "type" : "number",
          "description" : "Sum of gross income from agricultural, forestry, and livestock activities."
        },
        "grossIncomeIncreasesSum" : {
          "type" : "number",
          "description" : "Sum of gross income increases or adjustments."
        }
      }
    },
    "catC" : {
      "type" : "object",
      "description" : "Category C — Income from capital gains and other gains.",
      "properties" : {
        "periodNetIncome" : {
          "type" : "number",
          "description" : "Net income for the period from business and professional activities."
        }
      }
    },
    "catD" : {
      "type" : "object",
      "description" : "Category D — Income from capital.",
      "properties" : {
        "valueSum" : {
          "type" : "number",
          "description" : "Sum of income from capital yields or other category D sources."
        }
      }
    },
    "catE" : {
      "type" : "object",
      "description" : "Category E — Income subject to special and withholding rates.",
      "properties" : {
        "incomeSubjectToSpecialRates" : {
          "type" : "object",
          "description" : "Income subject to special taxation rates.",
          "properties" : {
            "totalIncome" : {
              "type" : "array",
              "description" : "Array of income amounts subject to special taxation rates.",
              "items" : {
                "type" : "number"
              }
            }
          }
        },
        "incomeSubjectToWithholdingRates" : {
          "type" : "object",
          "description" : "Income subject to withholding tax rates.",
          "properties" : {
            "totalIncome" : {
              "type" : "number",
              "description" : "Total income amount subject to withholding tax rates."
            },
            "totalWithholdingTax" : {
              "type" : "number",
              "description" : "Total amount of withholding tax applied to the income."
            }
          }
        }
      }
    },
    "catF" : {
      "type" : "object",
      "description" : "Category F — Income from property rental.",
      "properties" : {
        "grossAmountLeaseWithoutReduction" : {
          "type" : "number",
          "description" : "Gross income amount from lease contracts that do not benefit from the reduction regime."
        },
        "withholdingTaxLeaseWithoutReduction" : {
          "type" : "number",
          "description" : "Withholding tax applied to lease contracts that do not benefit from the reduction regime."
        },
        "grossAmountLeasePermanentHousing" : {
          "type" : "number",
          "description" : "Gross income amount from lease contracts for permanent housing."
        },
        "withholdingTaxLeasePermanentHousing" : {
          "type" : "number",
          "description" : "Withholding tax applied to lease contracts for permanent housing."
        },
        "grossAmountRealRightContract" : {
          "type" : "number",
          "description" : "Gross income amount from real right contracts."
        },
        "withholdingTaxRealRightContract" : {
          "type" : "number",
          "description" : "Withholding tax applied to real right contracts."
        }
      }
    },
    "catG" : {
      "type" : "object",
      "description" : "Category G — Income from asset disposals.",
      "properties" : {
        "realizationValueSum" : {
          "type" : "number",
          "description" : "Sum of realization values from the disposal of assets."
        },
        "acquisitionValueSum" : {
          "type" : "number",
          "description" : "Sum of acquisition values for the disposed assets."
        },
        "expensesAndChargesSum" : {
          "type" : "number",
          "description" : "Sum of expenses and charges related to the disposal of assets."
        }
      }
    },
    "catH" : {
      "type" : "object",
      "description" : "Category H — Other income including pensions and alimony.",
      "properties" : {
        "exemptIncomeSubjectToAggregation" : {
          "type" : "object",
          "description" : "Exempt income amounts that are still subject to aggregation for tax purposes.",
          "properties" : {
            "incomeSum" : {
              "type" : "number",
              "description" : "Total amount of exempt income subject to aggregation."
            },
            "personalIncomeTaxSum" : {
              "type" : "number",
              "description" : "Total amount of personal income tax associated with the exempt income."
            }
          }
        },
        "incomeFromIntellectualPropertySum" : {
          "type" : "number",
          "description" : "Sum of income received from intellectual property rights."
        },
        "alimonyPaymentSum" : {
          "type" : "number",
          "description" : "Sum of alimony payments made."
        },
        "taxBenefitsAndExpensesRelatedToPeopleWithDisabilities" : {
          "type" : "number",
          "description" : "Tax benefits and deductible expenses related to people with disabilities."
        }
      }
    },
    "catI" : {
      "type" : "object",
      "description" : "Category I — Income from certain specific activities and tax situations.",
      "properties" : {
        "simplifiedRegimeSum" : {
          "type" : "object",
          "description" : "Sum of values from simplified regime activities.",
          "properties" : {
            "grossIncome" : {
              "type" : "number",
              "description" : "Total gross income under the simplified taxation regime."
            },
            "netIncome" : {
              "type" : "number",
              "description" : "Total net income under the simplified taxation regime."
            }
          }
        },
        "incomeAllocationSum" : {
          "type" : "object",
          "description" : "Sum of income allocations for this category.",
          "properties" : {
            "commercialAndIndustrialIncome" : {
              "type" : "number",
              "description" : "Total income allocated from commercial and industrial activities."
            },
            "agriculturalForestryLivestockIncome" : {
              "type" : "number",
              "description" : "Total income allocated from agricultural, forestry, and livestock activities."
            }
          }
        },
        "localAccomodationIncomeSum" : {
          "type" : "number",
          "description" : "Total income amount from local accommodation activities."
        },
        "incurredAndPaidExpensesSum" : {
          "type" : "object",
          "description" : "Sum of incurred and paid expenses related to category I income.",
          "properties" : {
            "condominiumFees" : {
              "type" : "number",
              "description" : "Total amount of condominium fees paid."
            },
            "propertyTax" : {
              "type" : "number",
              "description" : "Total amount of property tax (IMI) paid."
            },
            "stampDuty" : {
              "type" : "number",
              "description" : "Total amount of stamp duty (Imposto do Selo) paid."
            },
            "municipalFees" : {
              "type" : "number",
              "description" : "Total amount of municipal fees paid."
            }
          }
        }
      }
    },
    "catJ" : {
      "type" : "array",
      "description" : "Category J — Income subject to optional aggregation, including foreign and miscellaneous income.",
      "items" : {
        "type" : "object",
        "properties" : {
          "employmentIncome" : {
            "type" : "object",
            "description" : "Income from employment, including wages and salaries.",
            "properties" : {
              "incomeSum" : {
                "type" : "number",
                "description" : "Total amount of employment income."
              },
              "socialProtectionContributionsSum" : {
                "type" : "number",
                "description" : "Total amount of social protection contributions deducted from employment income."
              },
              "taxPaidAbroadSum" : {
                "type" : "number",
                "description" : "Total amount of tax paid abroad on employment income."
              },
              "withholdingTaxSum" : {
                "type" : "number",
                "description" : "Total amount of withholding tax deducted from employment income."
              },
              "surchargeWithholdingSum" : {
                "type" : "number",
                "description" : "Total amount of surcharge withholding deducted from employment income."
              }
            }
          },
          "pensionIncome" : {
            "type" : "object",
            "description" : "Income from pensions.",
            "properties" : {
              "grossIncomeSum" : {
                "type" : "number",
                "description" : "Total gross income from pensions."
              },
              "socialProtectionContributionsSum" : {
                "type" : "number",
                "description" : "Total amount of social protection contributions deducted from pension income."
              },
              "taxPaidAbroadSum" : {
                "type" : "number",
                "description" : "Total amount of tax paid abroad on pension income."
              }
            }
          },
          "businessAndProfessionalIncome" : {
            "type" : "object",
            "description" : "Income from business and professional activities.",
            "properties" : {
              "incomeSum" : {
                "type" : "number",
                "description" : "Total income from business and professional activities."
              },
              "socialProtectionContributionsSum" : {
                "type" : "number",
                "description" : "Total social protection contributions deducted from business and professional income."
              },
              "taxPaidAbroadSum" : {
                "type" : "number",
                "description" : "Total amount of tax paid abroad on business and professional income."
              },
              "withholdingTaxInPortugalSum" : {
                "type" : "number",
                "description" : "Total amount of withholding tax deducted in Portugal on business and professional income."
              }
            }
          },
          "rentalIncome" : {
            "type" : "object",
            "description" : "Income from rental activities.",
            "properties" : {
              "netIncomeSum" : {
                "type" : "number",
                "description" : "Total net income from rental activities."
              }
            }
          },
          "capitalIncome" : {
            "type" : "object",
            "description" : "Income from capital sources.",
            "properties" : {
              "grossIncomeSum" : {
                "type" : "number",
                "description" : "Total gross income from capital sources."
              },
              "taxPaidAbroadInSourceCountrySum" : {
                "type" : "number",
                "description" : "Total amount of tax paid abroad in the source country on capital income."
              },
              "withheldTaxSum" : {
                "type" : "number",
                "description" : "Total amount of tax withheld at source on capital income."
              },
              "withholdingTaxInPortugalSum" : {
                "type" : "number",
                "description" : "Total amount of withholding tax deducted in Portugal on capital income."
              }
            }
          },
          "otherOptionalAggregationPatrimonialIncrements" : {
            "type" : "object",
            "description" : "Income from other patrimonial increments subject to optional aggregation.",
            "properties" : {
              "netIncomeSum" : {
                "type" : "number",
                "description" : "Total net income from other patrimonial increments subject to optional aggregation."
              }
            }
          }
        }
      }
    },
    "catL" : {
      "type" : "object",
      "description" : "Category L — Income details organized by type and source.",
      "properties" : {
        "dependentWorkIncome" : {
          "type" : "object",
          "description" : "Map of income from dependent work, keyed by description or code.",
          "additionalProperties" : {
            "type" : "object",
            "properties" : {
              "amount" : {
                "type" : "number",
                "description" : "Income amount."
              }
            }
          }
        },
        "simplifiedIncome" : {
          "type" : "object",
          "description" : "Map of income under the simplified regime, keyed by description or code.",
          "additionalProperties" : {
            "type" : "object",
            "properties" : {
              "amount" : {
                "type" : "number",
                "description" : "Income amount."
              }
            }
          }
        },
        "organizedIncome" : {
          "type" : "object",
          "description" : "Map of income under the organized accounting regime, keyed by description or code.",
          "additionalProperties" : {
            "type" : "object",
            "properties" : {
              "profit" : {
                "type" : "number",
                "description" : "Profit amount."
              },
              "loss" : {
                "type" : "number",
                "description" : "Loss amount."
              }
            }
          }
        },
        "imputedIncome" : {
          "type" : "object",
          "description" : "Map of imputed income, keyed by description or code.",
          "additionalProperties" : {
            "type" : "object",
            "properties" : {
              "amount" : {
                "type" : "number",
                "description" : "Income amount."
              }
            }
          }
        },
        "highValueIncome" : {
          "type" : "object",
          "description" : "Map of high-value foreign income, keyed by description or code.",
          "additionalProperties" : {
            "type" : "object",
            "properties" : {
              "boardFieldJ" : {
                "type" : "string",
                "description" : "Reference to the specific board field in section J of the form."
              },
              "amount" : {
                "type" : "number",
                "description" : "Income amount received from a foreign source."
              },
              "amountWithTax" : {
                "type" : "number",
                "description" : "Income amount from a foreign source after tax."
              },
              "foreignTaxed" : {
                "type" : "boolean",
                "description" : "Flag indicating whether the income was taxed abroad."
              }
            }
          }
        },
        "otherIncome" : {
          "type" : "object",
          "description" : "Map of other types of foreign income, keyed by description or code.",
          "additionalProperties" : {
            "type" : "object",
            "properties" : {
              "boardFieldJ" : {
                "type" : "string",
                "description" : "Reference to the specific board field in section J of the form."
              },
              "amount" : {
                "type" : "number",
                "description" : "Income amount received from a foreign source."
              },
              "amountWithTax" : {
                "type" : "number",
                "description" : "Income amount from a foreign source after tax."
              },
              "foreignTaxed" : {
                "type" : "boolean",
                "description" : "Flag indicating whether the income was taxed abroad."
              }
            }
          }
        }
      }
    }
  }
}

```