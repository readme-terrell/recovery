---
title: IRSByCode (Imposto sobre o Rendimento das Pessoas Singulares)
excerpt: Endpoint to retrieve the IRS document.
api:
  file: bizapis.json
  operationId: irs-imposto-sobre-o-rendimento-das-pessoas-singulares
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
> 💻 [block:html]{"html":"<h3  style=\"text-align:center;\">DOWNLOAD PROJECT</h3>\n<ul>\n  <li><a href=\"https://we.tl/t-3SOLdZPM9k\">Java</li>\n  <li><a href=\"https://we.tl/t-bGFxk8ahA5\">Python</li>\n  <li><a href=\"https://we.tl/t-RkPgchEPv7\">C#</li>\n</ul>\n<!--\n<a href=\"https://drive.google.com/uc?id=1MbJ3sWyhG8SqBhNYnmWcD9tcLvWGd2UK&export=download\">\n  <button>Download project demo</button>\n</a> -->"}[/block]

[block:html]
{
  "html": "<a href=\"https://www.bizapis.com/wp-content/uploads/2024/08/irs-by-code.mp4.mp4\" target=\"_blank\">To watch the video click here"
}
[/block]


# JSON Schema API Response

```json PT
{
  "type": "object",
  "properties": {
    "data": {
      "type": "object",
      "properties": {
        "requestId" : {
          "type" : "string",
          "description" : "Identificador único do pedido"
        }
      }
    },
    "file": {
      "type": "string",
      "description": "Ficheiro PDF em base 64"
    }
  }
}

```
```json ENG
{
  "type": "object",
  "properties": {
    "data": {
      "type": "object",
      "properties": {
        "requestId" : {
          "type" : "string",
          "description" : "Unique request identifier"
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