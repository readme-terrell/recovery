---
title: SS-SA (Segurança Social)
excerpt: The endpoint returns the current situation coming from Segurança Social
api:
  file: bizapis.json
  operationId: ss-sa-segurança-social
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
# JSON Schema API Response

```json PT
{
  "type" : "object",
  "properties" : {
    "requestId" : {
      "type" : "string",
      "description" : "Identificador único do pedido"
    },
    "total_values_to_receive" : {
      "type" : "string",
      "description" : "Valor total a receber"
    },
    "next_values_to_receive" : {
      "type" : "string",
      "description" : "Próximos valores a receber"
    },
    "values_not_received" : {
      "type" : "string",
      "description" : "Valores não recebidos"
    },
    "other_values_to_receive" : {
      "type" : "string",
      "description" : "Outros valores a receber"
    },
    "total_values_to_return_and_pay" : {
      "type" : "string",
      "description" : "Valores a devolver"
    },
    "notifications_for_value_restitution" : {
      "type" : "object",
      "description" : "Notificações para reposição de valor",
      "properties" : {
        "total" : {
          "type" : "string",
          "description" : "Valor total"
        },
        "color" : {
          "type" : "string",
          "description" : "Regra interna que adquire o valor de 'yellow' ou 'red' caso a regra se verifique e 'green' caso contrário"
        },
        "details" : {
          "type" : "array",
          "description" : "Lista de detalhes",
          "items" : {
            "type" : "object",
            "properties" : {
              "notification" : {
                "type" : "string",
                "description" : "O número de notificação"
              },
              "date" : {
                "type" : "string",
                "description" : "Data limite"
              },
              "value" : {
                "type" : "string",
                "description" : "Valor em euros"
              },
              "interest_value" : {
                "type" : "string",
                "description" : "Valor dos juros em euros"
              },
              "total_value" : {
                "type" : "string",
                "description" : "Valor total em euros"
              },
              "costs_value" : {
                "type" : "string",
                "description" : "Valor das custas em euros"
              },
              "fines_value" : {
                "type" : "string",
                "description" : "Valor das coimas em euros"
              },
              "message" : {
                "type" : "string",
                "description" : "Mensagem para casos onde não existem valores a apresentar"
              }
            }
          }
        }
      }
    },
    "other_values_to_return" : {
      "type" : "object",
      "$ref" : "urn:jsonschema:pt:infosistema:pojos:Note",
      "description" : "Outros valores a devolver"
    },
    "current_contributions" : {
      "type" : "object",
      "$ref" : "urn:jsonschema:pt:infosistema:pojos:Note",
      "description" : "Contribuições correntes"
    },
    "contributions_in_arrears" : {
      "type" : "object",
      "$ref" : "urn:jsonschema:pt:infosistema:pojos:Note",
      "description" : "Contribuições em atraso"
    },
    "fines_and_costs" : {
      "type" : "object",
      "$ref" : "urn:jsonschema:pt:infosistema:pojos:Note",
      "description" : "Coimas e custas"
    },
    "other_values_to_pay" : {
      "type" : "object",
      "$ref" : "urn:jsonschema:pt:infosistema:pojos:Note",
      "description" : "Outros valores a pagar"
    },
    "debt_in_fiscal_execution" : {
      "type" : "object",
      "$ref" : "urn:jsonschema:pt:infosistema:pojos:Note",
      "description" : "Dívida em execução fiscal"
    },
    "days_declaration_remunerations" : {
      "type" : "string",
      "description" : "Dias para declaração de remunerações"
    },
    "deadline_expired_declaration_remunerations" : {
      "type" : "string",
      "description" : "Prazo expirado para declaração de remunerações"
    },
    "days_tsu" : {
      "type" : "string",
      "description" : "Dias para Taxa Social Única (TSU)"
    },
    "deadline_expired_tsu" : {
      "type" : "string",
      "description" : "Prazo expirado para Taxa Social Única (TSU)"
    },
    "flag" : {
      "type" : "string",
      "description" : "Flag que pode adquirir o valor 'green' se todas as restantes regras estiverem 'green',  'red' se alguma das restantes regras estiver 'red' ou 'yellow' para qualquer outro caso"
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
      "description": "Unique request identifier"
    },
    "total_values_to_receive": {
      "type": "string",
      "description": "Total amount to receive"
    },
    "next_values_to_receive": {
      "type": "string",
      "description": "Upcoming amounts to receive"
    },
    "values_not_received": {
      "type": "string",
      "description": "Amounts not received"
    },
    "other_values_to_receive": {
      "type": "string",
      "description": "Other amounts to receive"
    },
    "total_values_to_return_and_pay": {
      "type": "string",
      "description": "Total amounts to return"
    },
    "notifications_for_value_restitution": {
      "type": "object",
      "description": "Notifications for value restitution",
      "properties": {
        "total": {
          "type": "string",
          "description": "Total amount"
        },
        "color": {
          "type": "string",
          "description": "Internal rule that acquires the value 'yellow' or 'red' if the rule applies, and 'green' otherwise"
        },
        "details": {
          "type": "array",
          "description": "List of details",
          "items": {
            "type": "object",
            "properties": {
              "notification": {
                "type": "string",
                "description": "Notification number"
              },
              "date": {
                "type": "string",
                "description": "Due date"
              },
              "value": {
                "type": "string",
                "description": "Amount in euros"
              },
              "interest_value": {
                "type": "string",
                "description": "Interest amount in euros"
              },
              "total_value": {
                "type": "string",
                "description": "Total amount in euros"
              },
              "costs_value": {
                "type": "string",
                "description": "Cost amount in euros"
              },
              "fines_value": {
                "type": "string",
                "description": "Fine amount in euros"
              },
              "message": {
                "type": "string",
                "description": "Message for cases where there are no amounts to display"
              }
            }
          }
        }
      }
    },
    "other_values_to_return": {
      "type": "object",
      "$ref": "urn:jsonschema:pt:infosistema:pojos:Note",
      "description": "Other amounts to return"
    },
    "current_contributions": {
      "type": "object",
      "$ref": "urn:jsonschema:pt:infosistema:pojos:Note",
      "description": "Current contributions"
    },
    "contributions_in_arrears": {
      "type": "object",
      "$ref": "urn:jsonschema:pt:infosistema:pojos:Note",
      "description": "Past due contributions"
    },
    "fines_and_costs": {
      "type": "object",
      "$ref": "urn:jsonschema:pt:infosistema:pojos:Note",
      "description": "Fines and costs"
    },
    "other_values_to_pay": {
      "type": "object",
      "$ref": "urn:jsonschema:pt:infosistema:pojos:Note",
      "description": "Other amounts to pay"
    },
    "debt_in_fiscal_execution": {
      "type": "object",
      "$ref": "urn:jsonschema:pt:infosistema:pojos:Note",
      "description": "Debt in fiscal execution"
    },
    "days_declaration_remunerations": {
      "type": "string",
      "description": "Days remaining for remuneration declaration"
    },
    "deadline_expired_declaration_remunerations": {
      "type": "string",
      "description": "Expired deadline for remuneration declaration"
    },
    "days_tsu": {
      "type": "string",
      "description": "Days remaining for Social Security Tax (TSU)"
    },
    "deadline_expired_tsu": {
      "type": "string",
      "description": "Expired deadline for Social Security Tax (TSU)"
    },
    "flag": {
      "type": "string",
      "description": "Flag that can acquire the value 'green' if all other rules are 'green', 'red' if any other rule is 'red', or 'yellow' for any other case"
    }
  }
}

```