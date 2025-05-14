---
title: CPRC (Certidão Permanente de Registo Comercial)
excerpt: >-
  CPRC ensures access to records and documents of any entity subject to
  commercial registration - companies, societies, cooperatives, public companies
  or others. This service replaced the now deprecated crc-service
api:
  file: bizapis.json
  operationId: cprc-certidão-permanente-de-registo-comercial
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
> 💻 [block:html]{"html":"<h3  style=\"text-align:center;\">DOWNLOAD PROJECT</h3>\n<ul>\n  <li><a href=\"https://we.tl/t-1AUtmd0FMl\">Java</li>\n  <li><a href=\"https://we.tl/t-ZpKo1qtEYo\">Python</li>\n  <li><a href=\"https://we.tl/t-gRrOI5AEjy\">C#</li>\n</ul>\n<!--\n<a href=\"https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download\">\n  <button>Download project demo</button>\n</a> -->"}[/block]

[block:html]
{
  "html": "<a href=\"https://www.bizapis.com/wp-content/uploads/2024/08/servico_certidao_permanente_reisto_comercial.mp4.mp4\" target=\"_blank\">To watch the video click here"
}
[/block]


# JSON Schema API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "request-id" : {
      "type" : "string",
      "description" : "Identificador único do pedido"
    },
    "client_id" : {
      "type" : "string",
      "description" : "Identificador do cliente que fez a solicitação"
    },
    "CRC" : {
      "type" : "string",
      "description" : "Código da Certidão Predial de Registo Comercial"
    },
    "NIPC" : {
      "type" : "string",
      "description" : "Número de Identificação de Pessoa Coletiva (NIPC) da empresa"
    },
    "titulo" : {
      "type" : "string",
      "description" : "Título do documento"
    },
    "NomeEmpresa" : {
      "type" : "string",
      "description" : "Nome da empresa"
    },
    "NaturezaJuridica" : {
      "type" : "string",
      "description" : "Natureza jurídica da empresa"
    },
    "MoradaSede" : {
      "type" : "object",
      "description" : "Endereço da sede da empresa",
      "properties" : {
        "Morada" : {
          "type" : "string",
          "description" : "Endereço completo da sede"
        },
        "Distrito" : {
          "type" : "string",
          "description" : "Distrito onde a sede está localizada"
        },
        "Concelho" : {
          "type" : "string",
          "description" : "Concelho onde a sede está localizada"
        },
        "Freguesia" : {
          "type" : "string",
          "description" : "Freguesia onde a sede está localizada"
        },
        "CodigoPostal" : {
          "type" : "string",
          "description" : "Código postal da sede"
        },
        "Localidade" : {
          "type" : "string",
          "description" : "Localidade onde a sede está localizada"
        }
      }
    },
    "CapitalSocial" : {
      "type" : "object",
      "description" : "Capital social da empresa",
      "properties" : {
        "Montante" : {
          "type" : "string",
          "description" : "Montante do capital social"
        },
        "Moeda" : {
          "type" : "string",
          "description" : "Moeda do capital social"
        },
        "Data" : {
          "type" : "string",
          "description" : "Data de registo do capital social"
        }
      }
    },
    "CAE" : {
      "type" : "object",
      "description" : "Código de Atividade Económica (CAE) da empresa",
      "properties" : {
        "Principal" : {
          "type" : "string",
          "description" : "CAE principal"
        },
        "Secundario" : {
          "type" : "array",
          "description" : "Lista CAE secundárias",
          "items" : {
            "type" : "string"
          }
        }
      }
    },
    "FormaObrigar" : {
      "type" : "string",
      "description" : "Forma como a empresa se obriga juridicamente"
    },
    "DataCriacao" : {
      "type" : "string",
      "description" : "Data de criação da empresa"
    },
    "DuracaoMandato" : {
      "type" : "string",
      "description" : "Duração do mandato dos órgãos sociais"
    },
    "DataFimMandato" : {
      "type" : "string",
      "description" : "Data de fim do mandato dos órgãos sociais"
    },
    "Representantes" : {
      "type" : "array",
      "description" : "Lista de representantes legais da empresa",
      "items" : {
        "type" : "object",
        "properties" : {
          "Nome" : {
            "type" : "string",
            "description" : "Nome do representante"
          },
          "NIFNIPC" : {
            "type" : "string",
            "description" : "Número de Identificação Fiscal (NIF) ou Número de Identificação de Pessoa Coletiva (NIPC)"
          },
          "Cargo" : {
            "type" : "string",
            "description" : "Cargo ou função do representante"
          },
          "BEF" : {
            "type" : "boolean",
            "description" : "Indica se o representante é beneficiário efetivo"
          },
          "PercentagemCapitalDetido" : {
            "type" : "string",
            "description" : "Percentagem do capital detido pelo representante"
          },
          "EstadoCivil" : {
            "type" : "string",
            "description" : "Estado civil do representante"
          },
          "NomeConjuge" : {
            "type" : "string",
            "description" : "Nome do cônjuge do representante"
          },
          "RegimeBens" : {
            "type" : "string",
            "description" : "Regime de bens aplicável ao representante"
          },
          "DataEntradaGerencia" : {
            "type" : "string",
            "description" : "Data de entrada na gerência"
          },
          "Sede" : {
            "type" : "object",
            "$ref" : "urn:jsonschema:pt:infosistema:bizapis:pojos:cprc:MoradaSede"
          }
        }
      }
    },
    "DataValidade" : {
      "type" : "string",
      "description" : "Data de validade da certidão"
    },
    "Socios" : {
      "type" : "object",
      "description" : "Informações sobre os sócios da empresa",
      "properties" : {
        "Unipessoal_SocioPessoaSingular" : {
          "type" : "string",
          "description" : "NIF do sócio pessoa singular no caso de ter a totalidade das quotas"
        },
        "Unipessoal_SocioPessoaColetiva" : {
          "type" : "string",
          "description" : "NIF do sócio pessoa coletiva no caso de ter a totalidade das quotas"
        },
        "SociosSingulares" : {
          "type" : "boolean",
          "description" : "Indica se a empresa tem sócios singulares"
        },
        "SociosColetivos" : {
          "type" : "boolean",
          "description" : "Indica se a empresa tem sócios coletivos"
        },
        "SociosSingulareseColetivos" : {
          "type" : "boolean",
          "description" : "Indica se a empresa tem tanto sócios singulares como coletivos"
        },
        "SociosGerentes" : {
          "type" : "array",
          "description" : "Lista de NIFs dos sócios gerentes",
          "items" : {
            "type" : "string"
          }
        },
        "ListaDeSocios" : {
          "type" : "array",
          "description" : "Lista de sócios da empresa",
          "items" : {
            "type" : "object",
            "properties" : {
              "Nome" : {
                "type" : "string",
                "description" : "Nome do sócio"
              },
              "NIFNIPC" : {
                "type" : "string",
                "description" : "Número de Identificação Fiscal (NIF) ou Número de Identificação de Pessoa Coletiva (NIPC)"
              },
              "EstadoCivil" : {
                "type" : "string",
                "description" : "Estado civil do sócio"
              },
              "ResidenciaSede" : {
                "type" : "string",
                "description" : "Residência ou sede do sócio"
              },
              "TipodeSocio" : {
                "type" : "string",
                "description" : "Tipo de sócio"
              },
              "Cargo" : {
                "type" : "string",
                "description" : "Cargo ou função do sócio"
              },
              "BEF" : {
                "type" : "boolean",
                "description" : "Indica se o sócio é beneficiário efetivo"
              },
              "SocioGerente" : {
                "type" : "boolean",
                "description" : "Indica se o sócio é gerente"
              },
              "PercentagemCapitalDetido" : {
                "type" : "string",
                "description" : "Percentagem do capital detido pelo sócio"
              },
              "ValorCapitalDetido" : {
                "type" : "string",
                "description" : "Valor do capital detido pelo sócio"
              }
            }
          }
        }
      }
    },
    "FactosPendentes" : {
      "type" : "boolean",
      "description" : "Indica se existem factos pendentes relacionados com a empresa"
    },
    "PenhoraQuotas" : {
      "type" : "boolean",
      "description" : "Indica se existe penhora de quotas na empresa"
    },
    "Penhor" : {
      "type" : "boolean",
      "description" : "Indica se existem penhores registados sobre a empresa"
    },
    "EmissaoObrigacoes" : {
      "type" : "boolean",
      "description" : "Indica se a empresa emitiu obrigações"
    },
    "ProcessoRevitalizacao" : {
      "type" : "boolean",
      "description" : "Indica se a empresa está em processo de revitalização"
    },
    "Objecto" : {
      "type" : "string",
      "description" : "Objeto social da empresa"
    },
    "Representantes_Gerentes" : {
      "type" : "array",
      "description" : "Lista de representantes gerentes da empresa",
      "items" : {
        "type" : "object",
        "properties" : {
          "Nome" : {
            "type" : "string",
            "description" : "Nome do representante gerente"
          },
          "NIFNIPC" : {
            "type" : "string",
            "description" : "Número de Identificação Fiscal (NIF) ou Número de Identificação de Pessoa Coletiva (NIPC)"
          }
        }
      }
    },
    "NumeroRepresentantesGerentes" : {
      "type" : "integer",
      "description" : "Número total de representantes gerentes"
    },
    "PoderesDeAssinatura" : {
      "type" : "object",
      "description" : "Informações sobre os poderes de assinatura na empresa",
      "properties" : {
        "ObrigaCom1Assinatura" : {
          "type" : "array",
          "description" : "Lista composta por Número de Identificação Fiscal (NIF) ou Número de Identificação de Pessoa Coletiva (NIPC) quando existe apenas uma pessoa responsável pela assinatura",
          "items" : {
            "type" : "string"
          }
        },
        "ObrigaCom2Assinaturas" : {
          "type" : "array",
          "description" : "Lista composta por Número de Identificação Fiscal (NIF) ou Número de Identificação de Pessoa Coletiva (NIPC) quando existem duas pessoas responsáveis pela assinatura",
          "items" : {
            "type" : "string"
          }
        }
      }
    },
    "Tem_Erro_Leitura" : {
      "type" : "boolean",
      "description" : "Indica se houve erro na leitura da certidão"
    },
    "SociedadeAnonima" : {
      "type" : "boolean"
    },
    "SociedadePorQuotas" : {
      "type" : "boolean"
    }
  }
}
```
```json ENG
{
  "type": "object",
  "properties": {
    "request-id": {
      "type": "string",
      "description": "Unique request identifier"
    },
    "client_id": {
      "type": "string",
      "description": "Identifier of the client who made the request"
    },
    "CRC": {
      "type": "string",
      "description": "Commercial Registry Certificate Code"
    },
    "NIPC": {
      "type": "string",
      "description": "Corporate Tax Identification Number (NIPC) of the company"
    },
    "titulo": {
      "type": "string",
      "description": "Title of the document"
    },
    "NomeEmpresa": {
      "type": "string",
      "description": "Company name"
    },
    "NaturezaJuridica": {
      "type": "string",
      "description": "Legal nature of the company"
    },
    "MoradaSede": {
      "type": "object",
      "description": "Company headquarters address",
      "properties": {
        "Morada": {
          "type": "string",
          "description": "Full address of the headquarters"
        },
        "Distrito": {
          "type": "string",
          "description": "District where the headquarters is located"
        },
        "Concelho": {
          "type": "string",
          "description": "Municipality where the headquarters is located"
        },
        "Freguesia": {
          "type": "string",
          "description": "Parish where the headquarters is located"
        },
        "CodigoPostal": {
          "type": "string",
          "description": "Postal code of the headquarters"
        },
        "Localidade": {
          "type": "string",
          "description": "Locality where the headquarters is located"
        }
      }
    },
    "CapitalSocial": {
      "type": "object",
      "description": "Company's share capital",
      "properties": {
        "Montante": {
          "type": "string",
          "description": "Amount of share capital"
        },
        "Moeda": {
          "type": "string",
          "description": "Currency of the share capital"
        },
        "Data": {
          "type": "string",
          "description": "Date of share capital registration"
        }
      }
    },
    "CAE": {
      "type": "object",
      "description": "Company's Economic Activity Code (CAE)",
      "properties": {
        "Principal": {
          "type": "string",
          "description": "Primary CAE"
        },
        "Secundario": {
          "type": "array",
          "description": "List of secondary CAEs",
          "items": {
            "type": "string"
          }
        }
      }
    },
    "FormaObrigar": {
      "type": "string",
      "description": "How the company is legally bound"
    },
    "DataCriacao": {
      "type": "string",
      "description": "Company's creation date"
    },
    "DuracaoMandato": {
      "type": "string",
      "description": "Term duration of the governing bodies"
    },
    "DataFimMandato": {
      "type": "string",
      "description": "End date of the governing bodies' term"
    },
    "Representantes": {
      "type": "array",
      "description": "List of the company's legal representatives",
      "items": {
        "type": "object",
        "properties": {
          "Nome": {
            "type": "string",
            "description": "Representative's name"
          },
          "NIFNIPC": {
            "type": "string",
            "description": "Tax Identification Number (NIF) or Corporate Tax Identification Number (NIPC)"
          },
          "Cargo": {
            "type": "string",
            "description": "Representative's position or role"
          },
          "BEF": {
            "type": "boolean",
            "description": "Indicates if the representative is a beneficial owner"
          },
          "PercentagemCapitalDetido": {
            "type": "string",
            "description": "Percentage of capital held by the representative"
          },
          "EstadoCivil": {
            "type": "string",
            "description": "Representative's marital status"
          },
          "NomeConjuge": {
            "type": "string",
            "description": "Representative's spouse name"
          },
          "RegimeBens": {
            "type": "string",
            "description": "Representative's marital property regime"
          },
          "DataEntradaGerencia": {
            "type": "string",
            "description": "Date of entry into management"
          },
          "Sede": {
            "type": "object",
            "$ref": "urn:jsonschema:pt:infosistema:bizapis:pojos:cprc:MoradaSede"
          }
        }
      }
    },
    "DataValidade": {
      "type": "string",
      "description": "Certificate's validity date"
    },
    "FactosPendentes": {
      "type": "boolean",
      "description": "Indicates if there are pending facts related to the company"
    },
    "PenhoraQuotas": {
      "type": "boolean",
      "description": "Indicates if there is a seizure of company shares"
    },
    "Penhor": {
      "type": "boolean",
      "description": "Indicates if there are registered pledges over the company"
    },
    "EmissaoObrigacoes": {
      "type": "boolean",
      "description": "Indicates if the company has issued bonds"
    },
    "ProcessoRevitalizacao": {
      "type": "boolean",
      "description": "Indicates if the company is undergoing a revitalization process"
    },
    "Objecto": {
      "type": "string",
      "description": "Company's corporate purpose"
    },
    "Representantes_Gerentes": {
      "type": "array",
      "description": "List of the company's managing representatives",
      "items": {
        "type": "object",
        "properties": {
          "Nome": {
            "type": "string",
            "description": "Managing representative's name"
          },
          "NIFNIPC": {
            "type": "string",
            "description": "Tax Identification Number (NIF) or Corporate Tax Identification Number (NIPC)"
          }
        }
      }
    },
    "NumeroRepresentantesGerentes": {
      "type": "integer",
      "description": "Total number of managing representatives"
    },
    "PoderesDeAssinatura": {
      "type": "object",
      "description": "Information about the company's signing authority",
      "properties": {
        "ObrigaCom1Assinatura": {
          "type": "array",
          "description": "List of Tax Identification Numbers (NIF) or Corporate Tax Identification Numbers (NIPC) when there is only one person responsible for signing",
          "items": {
            "type": "string"
          }
        },
        "ObrigaCom2Assinaturas": {
          "type": "array",
          "description": "List of Tax Identification Numbers (NIF) or Corporate Tax Identification Numbers (NIPC) when two people are responsible for signing",
          "items": {
            "type": "string"
          }
        }
      }
    },
    "Tem_Erro_Leitura": {
      "type": "boolean",
      "description": "Indicates if there was an error in reading the certificate"
    },
    "SociedadeAnonima": {
      "type": "boolean"
    },
    "SociedadePorQuotas": {
      "type": "boolean"
    }
  }
}

```