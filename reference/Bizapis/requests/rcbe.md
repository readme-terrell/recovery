---
title: RCBE (Registo Central do Beneficiário Efetivo)
excerpt: >-
  The RCBE enables identify all people that control a fund, company or legal
  entities of another nature. The purpose of this endpoint, is to consult the
  RCBE declaration.
api:
  file: bizapis.json
  operationId: rcbe
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
> 💻 <HTMLBlock>{`
> <h3  style="text-align:center;">DOWNLOAD PROJECT</h3>
> <ul>
>   <li><a href="https://we.tl/t-SrT6D63DQy">Java</li>
>   <li><a href="https://we.tl/t-sNKn0t88Ix">Python</li>
>   <li><a href="https://we.tl/t-i5pJvRhWo5">C#</li>
> </ul>
> `}</HTMLBlock>

## Timeout after 30 seconds

In case this service doesn't present a response during the period of 30 seconds, the API will respond with the following response body:

```json json
{
    "data": "44c8f08c-bc29-43a2-81c8-5541873ca2c2"
}
```

This value can be used as the path parameter (requestId) in this [endpoint ](https://bizapis.readme.io/reference/retrieve-persistent-data) in order to retrieve the stored data.

<HTMLBlock>{`
<a href="https://www.bizapis.com/wp-content/uploads/2024/08/Servico_RCBE.mp4.mp4" target="_blank">To watch the video click here
`}</HTMLBlock>

# JSON Schema API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "RequestId" : {
      "type" : "string",
      "description" : "Identificador único do pedido."
    },
    "Entidade Sujeita" : {
      "type" : "object",
      "description" : "Informações detalhadas sobre a entidade sujeita ao Registio Comercial Beneficiário Efetivo.",
      "properties" : {
        "Firma ou denominação" : {
          "type" : "string",
          "description" : "Nome da firma ou denominação social da entidade sujeita."
        },
        "NIF" : {
          "type" : "string",
          "description" : "Número de Identificação Fiscal (NIF) da entidade."
        },
        "País de residência" : {
          "type" : "string",
          "description" : "País de residência da entidade sujeita."
        },
        "Natureza Jurídica" : {
          "type" : "string",
          "description" : "Natureza jurídica da entidade."
        },
        "CAE" : {
          "type" : "string",
          "description" : "Código de Atividade Económica (CAE) da entidade."
        },
        "Identificador entidades jurídicas" : {
          "type" : "string",
          "description" : "Identificador único da entidade jurídica."
        },
        "Morada" : {
          "type" : "string",
          "description" : "Morada da sede ou do estabelecimento da entidade."
        },
        "Distrito" : {
          "type" : "string",
          "description" : "Distrito onde a entidade está localizada."
        },
        "Concelho" : {
          "type" : "string",
          "description" : "Concelho onde a entidade está localizada."
        },
        "Freguesia" : {
          "type" : "string",
          "description" : "Freguesia onde a entidade está localizada."
        },
        "Endereço eletrónico institucional" : {
          "type" : "string",
          "description" : "Endereço eletrónico institucional da entidade."
        }
      }
    },
    "Dados Beneficiario" : {
      "type" : "array",
      "description" : "Lista com os dados dos beneficiários efetivos associados à entidade.",
      "items" : {
        "type" : "object",
        "properties" : {
          "nome" : {
            "type" : "string",
            "description" : "Nome do beneficiário."
          },
          "apelido" : {
            "type" : "string",
            "description" : "Apelido do beneficiário."
          },
          "data nascimento" : {
            "type" : "string",
            "description" : "Data de nascimento do beneficiário (formato: DD/MM/YYYY)."
          },
          "nacionalidade" : {
            "type" : "string",
            "description" : "Nacionalidade do beneficiário."
          },
          "fonte de informação" : {
            "type" : "string",
            "description" : "Fonte da informação sobre o beneficiário."
          },
          "menor de idade" : {
            "type" : "string",
            "description" : "Indica se o beneficiário é menor de idade (sim ou não)."
          },
          "maior acompanhado" : {
            "type" : "string",
            "description" : "Indica se o beneficiário é maior de idade, mas acompanhado (sim ou não)."
          },
          "Interesse Detido" : {
            "type" : "object",
            "description" : "Informações sobre o interesse detido pelo beneficiário.",
            "properties" : {
              "benefeciario" : {
                "type" : "string",
                "description" : "Nome do beneficiário que detém o interesse na entidade."
              },
              "proprietario" : {
                "type" : "string",
                "description" : "Indicação se é proprietário da entidade ou do ativo."
              },
              "tipo de ativos" : {
                "type" : "string",
                "description" : "Tipo de ativos detidos."
              },
              "capital social" : {
                "type" : "string",
                "description" : "Percentagem do capital social detido pelo beneficiário ou proprietário."
              },
              "tipo de detenção" : {
                "type" : "string",
                "description" : "Tipo de detenção do ativo."
              },
              "estrutura da detenção" : {
                "type" : "string",
                "description" : "Estrutura da detenção do ativo."
              },
              "direitos de voto" : {
                "type" : "string",
                "description" : "Indicação dos direitos de voto associados ao ativo detido (sim ou não)."
              },
              "controlo sobre a entidade" : {
                "type" : "string",
                "description" : "Indica o controlo sobre a entidade pelo beneficiário ou proprietário (sim ou não)."
              },
              "direção da entidade" : {
                "type" : "string",
                "description" : "Indicação de se o beneficiário ou proprietário exerce funções na direção da entidade (sim ou não)."
              },
              "fundador da entidade" : {
                "type" : "string",
                "description" : "Indica se o beneficiário ou proprietário é fundador da entidade."
              },
              "administrador da entidade" : {
                "type" : "string",
                "description" : "Indica se o beneficiário ou proprietário é administrador da entidade."
              },
              "controlo final sobre a entidade" : {
                "type" : "string",
                "description" : "Indica se o beneficiário ou proprietário exerce controlo final sobre a entidade."
              },
              "curador da entidade" : {
                "type" : "string",
                "description" : "Indica se o beneficiário ou proprietário é curador da entidade."
              },
              "pertence a categoria fundador, administrador ou curador" : {
                "type" : "string",
                "description" : "Indica a categoria do beneficiário ou proprietário."
              },
              "fonte informação" : {
                "type" : "string",
                "description" : "Fonte da informação sobre o interesse detido."
              }
            }
          }
        }
      }
    },
    "Submissão" : {
      "type" : "object",
      "description" : "Informações sobre o estado e data da submissão.",
      "properties" : {
        "Data de submissão" : {
          "type" : "string",
          "description" : "Data em que a submissão foi realizada."
        },
        "Estado da submissão" : {
          "type" : "string",
          "description" : "Estado atual da submissão."
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
    "RequestId": {
      "type": "string",
      "description": "Unique identifier for the request."
    },
    "Entidade Sujeita": {
      "type": "object",
      "description": "Detailed information about the entity subject to the Beneficial Ownership Registry (RCBE).",
      "properties": {
        "Firma ou denominação": {
          "type": "string",
          "description": "The name of the entity or its registered business name."
        },
        "NIF": {
          "type": "string",
          "description": "The Tax Identification Number (NIF) of the entity."
        },
        "País de residência": {
          "type": "string",
          "description": "The country of residence of the entity."
        },
        "Natureza Jurídica": {
          "type": "string",
          "description": "The legal nature of the entity."
        },
        "CAE": {
          "type": "string",
          "description": "The Economic Activity Code (CAE) of the entity."
        },
        "Identificador entidades jurídicas": {
          "type": "string",
          "description": "The unique identifier of the legal entity."
        },
        "Morada": {
          "type": "string",
          "description": "The physical address of the entity's headquarters or establishment."
        },
        "Distrito": {
          "type": "string",
          "description": "The district where the entity is located."
        },
        "Concelho": {
          "type": "string",
          "description": "The municipality where the entity is located."
        },
        "Freguesia": {
          "type": "string",
          "description": "The parish where the entity is located."
        },
        "Endereço eletrónico institucional": {
          "type": "string",
          "description": "The institutional email address of the entity."
        }
      }
    },
    "Dados Beneficiario": {
      "type": "array",
      "description": "A list of the beneficial owners associated with the entity.",
      "items": {
        "type": "object",
        "properties": {
          "nome": {
            "type": "string",
            "description": "The first name of the beneficial owner."
          },
          "apelido": {
            "type": "string",
            "description": "The surname of the beneficial owner."
          },
          "data nascimento": {
            "type": "string",
            "description": "The date of birth of the beneficial owner (format: DD/MM/YYYY)."
          },
          "nacionalidade": {
            "type": "string",
            "description": "The nationality of the beneficial owner."
          },
          "fonte de informação": {
            "type": "string",
            "description": "The source of information about the beneficial owner."
          },
          "menor de idade": {
            "type": "string",
            "description": "Indicates whether the beneficial owner is a minor (yes or no)."
          },
          "maior acompanhado": {
            "type": "string",
            "description": "Indicates whether the beneficial owner is an adult but is accompanied (yes or no)."
          },
          "Interesse Detido": {
            "type": "object",
            "description": "Information about the interest held by the beneficial owner.",
            "properties": {
              "benefeciario": {
                "type": "string",
                "description": "The name of the beneficial owner holding the interest in the entity."
              },
              "proprietario": {
                "type": "string",
                "description": "Indicates whether the beneficial owner is also the owner of the entity or the asset."
              },
              "tipo de ativos": {
                "type": "string",
                "description": "The type of assets held by the beneficial owner."
              },
              "capital social": {
                "type": "string",
                "description": "The percentage of the entity's capital held by the beneficial owner or proprietor."
              },
              "tipo de detenção": {
                "type": "string",
                "description": "The type of ownership or holding of the asset."
              },
              "estrutura da detenção": {
                "type": "string",
                "description": "The structure of asset ownership."
              },
              "direitos de voto": {
                "type": "string",
                "description": "Indicates whether the beneficial owner holds voting rights on the asset (yes or no)."
              },
              "controlo sobre a entidade": {
                "type": "string",
                "description": "Indicates whether the beneficial owner exercises control over the entity (yes or no)."
              },
              "direção da entidade": {
                "type": "string",
                "description": "Indicates whether the beneficial owner holds a position in the entity's management (yes or no)."
              },
              "fundador da entidade": {
                "type": "string",
                "description": "Indicates whether the beneficial owner is a founder of the entity."
              },
              "administrador da entidade": {
                "type": "string",
                "description": "Indicates whether the beneficial owner is an administrator of the entity."
              },
              "controlo final sobre a entidade": {
                "type": "string",
                "description": "Indicates whether the beneficial owner has final control over the entity."
              },
              "curador da entidade": {
                "type": "string",
                "description": "Indicates whether the beneficial owner is a curator of the entity."
              },
              "pertence a categoria fundador, administrador ou curador": {
                "type": "string",
                "description": "Indicates the category of the beneficial owner."
              },
              "fonte informação": {
                "type": "string",
                "description": "The source of the information about the interest held."
              }
            }
          }
        }
      }
    },
    "Submissão": {
      "type": "object",
      "description": "Information regarding the submission status and date.",
      "properties": {
        "Data de submissão": {
          "type": "string",
          "description": "The date on which the submission was made."
        },
        "Estado da submissão": {
          "type": "string",
          "description": "The current status of the submission."
        }
      }
    }
  }
}

```