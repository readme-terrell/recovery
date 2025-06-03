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

* [Java](https://we.tl/t-joAUO6NZlJ)
* [Python](https://we.tl/t-RMtHpM3KKU)
* [C#](https://we.tl/t-0rXaS2WgvY)

[Watch the video](https://www.bizapis.com/wp-content/uploads/2024/08/servico-irs_by_user_password.mp4.mp4)

# JSON Schema for API Response

```json
{
  "type" : "object",
  "properties" : {
    "requestId" : {
      "type" : "string"
    },
    "intro" : {
      "type" : "object",
      "properties" : {
        "yearOfIncome" : {
          "type" : "string"
        },
        "taxpayerNIFA" : {
          "type" : "string"
        },
        "taxpayerNIFB" : {
          "type" : "string"
        }
      }
    },
    "catA" : {
      "type" : "object",
      "properties" : {
        "incomeFromDependentWorkSum" : {
          "type" : "number"
        },
        "withholdingTaxSum" : {
          "type" : "number"
        },
        "contributionsSum" : {
          "type" : "number"
        },
        "surtaxWithholdingSum" : {
          "type" : "number"
        },
        "unionDuesSum" : {
          "type" : "number"
        }
      }
    },
    "catB" : {
      "type" : "object",
      "properties" : {
        "grossProfessionalCommercialAndIndustrialIncomeSum" : {
          "type" : "number"
        },
        "grossAgriculturalForestryAndLivestockIncomeSum" : {
          "type" : "number"
        },
        "grossIncomeIncreasesSum" : {
          "type" : "number"
        }
      }
    },
    "catC" : {
      "type" : "object",

      "properties" : {
        "periodNetIncome" : {
          "type" : "number"
        }
      }
    },
    "catD" : {
      "type" : "object",

      "properties" : {
        "valueSum" : {
          "type" : "number"
        }
      }
    },
    "catE" : {
      "type" : "object",
      "properties" : {
        "incomeSubjectToSpecialRates" : {
          "type" : "object",
          "properties" : {
            "totalIncome" : {
              "type" : "array",
              "items" : {
                "type" : "number"
              }
            }
          }
        },
        "incomeSubjectToWithholdingRates" : {
          "type" : "object",
          "properties" : {
            "totalIncome" : {
              "type" : "number"
            },
            "totalWithholdingTax" : {
              "type" : "number"
            }
          }
        }
      }
    },
    "catF" : {
      "type" : "object",
      "properties" : {
        "grossAmountLeaseWithoutReduction" : {
          "type" : "number"
        },
        "withholdingTaxLeaseWithoutReduction" : {
          "type" : "number"
        },
        "grossAmountLeasePermanentHousing" : {
          "type" : "number"
        },
        "withholdingTaxLeasePermanentHousing" : {
          "type" : "number"
        },
        "grossAmountRealRightContract" : {
          "type" : "number"
        },
        "withholdingTaxRealRightContract" : {
          "type" : "number"
        }
      }
    },
    "catG" : {
      "type" : "object",
      "properties" : {
        "realizationValueSum" : {
          "type" : "number"
        },
        "acquisitionValueSum" : {
          "type" : "number"
        },
        "expensesAndChargesSum" : {
          "type" : "number"
        }
      }
    },
    "catH" : {
      "type" : "object",
      "properties" : {
        "exemptIncomeSubjectToAggregation" : {
          "type" : "object",
          "properties" : {
            "incomeSum" : {
              "type" : "number"
            },
            "personalIncomeTaxSum" : {
              "type" : "number"
            }
          }
        },
        "incomeFromIntellectualPropertySum" : {
          "type" : "number"
        },
        "alimonyPaymentSum" : {
          "type" : "number"
        },
        "taxBenefitsAndExpensesRelatedToPeopleWithDisabilities" : {
          "type" : "number"
        }
      }
    },
    "catI" : {
      "type" : "object",
      "properties" : {
        "simplifiedRegimeSum" : {
          "type" : "object",
          "properties" : {
            "grossIncome" : {
              "type" : "number"
            },
            "netIncome" : {
              "type" : "number"
            }
          }
        },
        "incomeAllocationSum" : {
          "type" : "object",
          "properties" : {
            "commercialAndIndustrialIncome" : {
              "type" : "number"
            },
            "agriculturalForestryLivestockIncome" : {
              "type" : "number"
            }
          }
        },
        "localAccomodationIncomeSum" : {
          "type" : "number"
        },
        "incurredAndPaidExpensesSum" : {
          "type" : "object",

          "properties" : {
            "condominiumFees" : {
              "type" : "number"
            },
            "propertyTax" : {
              "type" : "number"
            },
            "stampDuty" : {
              "type" : "number"
            },
            "municipalFees" : {
              "type" : "number"
            }
          }
        }
      }
    },
    "catJ" : {
      "type" : "object",
      "properties" : {
        "employmentIncome" : {
          "type" : "object",
          "properties" : {
            "incomeSum" : {
              "type" : "number"
            },
            "socialProtectionContributionsSum" : {
              "type" : "number"
            },
            "taxPaidAbroadSum" : {
              "type" : "number"
            },
            "withholdingTaxSum" : {
              "type" : "number"
            },
            "surchargeWithholdingSum" : {
              "type" : "number"
            }
          }
        },
        "pensionIncome" : {
          "type" : "object",
          "properties" : {
            "grossIncomeSum" : {
              "type" : "number"
            },
            "socialProtectionContributionsSum" : {
              "type" : "number"
            },
            "taxPaidAbroadSum" : {
              "type" : "number"
            }
          }
        },
        "businessAndProfessionalIncome" : {
          "type" : "object",
          "properties" : {
            "incomeSum" : {
              "type" : "number"
            },
            "socialProtectionContributionsSum" : {
              "type" : "number"
            },
            "taxPaidAbroadSum" : {
              "type" : "number"
            },
            "withholdingTaxInPortugalSum" : {
              "type" : "number"
            }
          }
        },
        "rentalIncome" : {
          "type" : "object",
          "properties" : {
            "netIncomeSum" : {
              "type" : "number"
            }
          }
        },
        "capitalIncome" : {
          "type" : "object",
          "properties" : {
            "grossIncomeSum" : {
              "type" : "number"
            },
            "taxPaidAbroadInSourceCountrySum" : {
              "type" : "number"
            },
            "withheldTaxSum" : {
              "type" : "number"
            },
            "withholdingTaxInPortugalSum" : {
              "type" : "number"
            }
          }
        },
        "otherOptionalAggregationPatrimonialIncrements" : {
          "type" : "object",
          "properties" : {
            "netIncomeSum" : {
              "type" : "number"
            }
          }
        }
      }
    },
    "catL" : {
      "type" : "object",
      "properties" : {
        "dependentWorkIncome" : {
          "type" : "object",
          "additionalProperties" : {
            "type" : "object",
            "properties" : {
              "amount" : {
                "type" : "number"
              }
            }
          }
        },
        "simplifiedIncome" : {
          "type" : "object",
          "additionalProperties" : {
            "type" : "object",
            "$ref" : "urn:jsonschema:pt:infosistema:irs_by_user_password_details_service:pojo:cat_l:Income"
          }
        },
        "organizedIncome" : {
          "type" : "object",
          "additionalProperties" : {
            "type" : "object",
            "properties" : {
              "profit" : {
                "type" : "number"
              },
              "loss" : {
                "type" : "number"
              }
            }
          }
        },
        "imputedIncome" : {
          "type" : "object",
          "additionalProperties" : {
            "type" : "object",
            "$ref" : "urn:jsonschema:pt:infosistema:irs_by_user_password_details_service:pojo:cat_l:Income"
          }
        },
        "highValueIncome" : {
          "type" : "object",
          "additionalProperties" : {
            "type" : "object",
            "properties" : {
              "boardFieldJ" : {
                "type" : "string"
              },
              "amount" : {
                "type" : "number"
              },
              "amountWithTax" : {
                "type" : "number"
              },
              "foreignTaxed" : {
                "type" : "boolean"
              }
            }
          }
        },
        "otherIncome" : {
          "type" : "object",
          "additionalProperties" : {
            "type" : "object",
            "$ref" : "urn:jsonschema:pt:infosistema:irs_by_user_password_details_service:pojo:cat_l:ForeignIncome"
          }
        }
      }
    }
  }
}
```