---
title: AT-Alerts (Autoridade Tributária Alertas)
excerpt: Endpoint to retrieve the list of alerts in Autoridade Tributária.
api:
  file: bizapis.json
  operationId: at-alerts
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

<div style={{ textAlign: "center" }}>
  <h3>DOWNLOAD PROJECT</h3>
</div>

- [Java](https://we.tl/t-Rn1fLb7De5)
- [Python](https://we.tl/t-IzIyzBXPgd)
- [C#](https://we.tl/t-NJGCT18utw)

<a href="https://www.bizapis.com/wp-content/uploads/2024/08/servico_autoridade_tributaria_alerts.mp4.mp4" target="_blank">
  To watch the video click here
</a>

# JSON Schema API Response

## Portuguese

```json
{
  "type" : "object",
  "properties" : {
    "requestId" : {
      "type" : "string",
      "description" : "Identificador único do pedido."
    },
    "alerts" : {
      "type" : "array",
      "description" : "Lista de alertas emitidos pela Autoridade Tributária. Pode incluir prazos de pagamento, avisos de irregularidades ou necessidade de submissão de declarações.",
      "items" : {
        "type" : "object",
        "properties" : {
          "descriptionName" : {
            "type" : "string",
            "description" : "O nome ou categoria do alerta."
          },
          "description" : {
            "type" : "string",
            "description" : "Uma explicação detalhada sobre o alerta."
          },
          "limitDate" : {
            "type" : "string",
            "description" : "O prazo ou data em que a ação associada ao alerta deve ser concluída, no formato 'YYYY-MM-DD'."
          }
        }
      }
    }
  }
}
```

## English

```json
{
  "type": "object",
  "properties": {
    "requestId": {
      "type": "string",
      "description": "Unique identifier for the request."
    },
    "alerts": {
      "type": "array",
      "description": "List of alerts issued by the Tax Authority. This may include payment deadlines, notices of irregularities, or the need for declaration submissions.",
      "items": {
        "type": "object",
        "properties": {
          "descriptionName": {
            "type": "string",
            "description": "The name or category of the alert."
          },
          "description": {
            "type": "string",
            "description": "A detailed explanation about the alert."
          },
          "limitDate": {
            "type": "string",
            "description": "The deadline or date by which the action associated with the alert must be completed, in the format 'YYYY-MM-DD'."
          }
        }
      }
    }
  }
}
```