---
title: Starting Guide
excerpt: ''
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
# bizAPIs Documentation

bizAPIs is a solution that assists companies in automating their processes, allowing access to external data such as standards and market information, etc. Moreover, it keeps companies up-to-date with changes, making operations more efficient and secure to make more informed decisions.

This page aims to provide guidance to facilitate the integration process of data coming from our bizAPIs product API and to explain some specific features of the product.

## Workflow

<Image align="center" src="https://files.readme.io/efa70198c0c071c113489e5c0a7ec62cc02e35d973676f4e099857776e6e5cb6-RequestWorkflow.drawio.png" />

## Subscriptions (API Key)

To make requests to the bizAPIs API, it is necessary for the developer to have an API key (or, as we call it, a subscription).

The subscription is responsible for identifying the user and persisting information about which services (endpoints) the developer has access to.

Registration for each of the services is individual, and at this moment, the developer has to make a request to our team using this [contact form](https://www.bizapis.com/contact-sales/).

## Mock data

Most of the services currently have mock data to ensure that developers can perform simulations of the requests during the initial phases of integration with the API, restricting access to real data.

All requests made with the API Key provided in the documentation are solely and exclusively intended for the test data.

If there is an interest in moving to an integration using real data, get in touch with us using this [contact form](https://www.bizapis.com/contact-sales/).

## Contacts

For more information about the product, you can visit our [website](https://www.bizapis.com/), or get in touch with us using this [contact form](https://www.bizapis.com/contact-sales/).

## How Make a Request

Each API contains essential documentation that provides necessary information about the endpoints, the API Key, parameters, and the available responses.

### Test in Postman:

![Postman URL](https://files.readme.io/7dc2c99-url_Postman.png)

* Set up the URL:
  1. Select the POST method.
  2. The specific URL for each endpoint is provided in the documentation for each API. Copy the URL corresponding to the desired endpoint.

![URL Example](https://files.readme.io/1ff69f6-urlsublinhado.png)

<br />

<br />

![Authorization](https://files.readme.io/bf0819a-Authorization.png)

* Set up Authorization:
  1. Go to the "Authorization" tab in Postman.
  2. In the "Type" field, select "Bearer Token".
  3. Paste the API Key into the "Token" field.

![Authorization Example](https://files.readme.io/4b3c0d2-autorizaaosublinhada.png)

<br />

<br />

![Request Body](https://files.readme.io/0443e8c-body_Request.png)

* Set up Request Body:
  1. In Postman, select the "Body" tab
  2. Choose the "raw" option.
  3. Ensure the selected format is "JSON".
  4. Copy the requestBody according to the format specified in the API documentation.

![Request Body Example](https://files.readme.io/96a09ab-requestbodysublinhado.png)

<br />

<br />

![Response](https://files.readme.io/32e43de-response.png)

* Send the request:
  1. After setting up the URL, authorization, and request body, click the "Send" button to send the request to the API. By following these steps, you will be ready to start interacting with the API.

## HTTP Status Code

| Status Code | Message Code          |
| :---------- | :-------------------- |
| 200         | OK                    |
| 401         | Unauthorized          |
| 429         | Too many requests     |
| 500         | Internal Server Error |
| 503         | Service Unavailable   |
| 504         | Gateway Timeout       |

**Important:**

For 200 HTTP Codes, in case of error, the response body contains the field '**messageStatusCode**'.

This field is composed by the **service\_code** + **bizapis\_error\_code**

Ex: 001\_011 corresponds to, error in service AT-Aggregator - Fail to login website Timeout

## Service "Names" Codes

|     |                          |
| :-- | :----------------------- |
| 001 | AT-Aggregator            |
| 002 | AT-Alert                 |
| 003 | AT-Divida                |
| 004 | AT-Interacoes            |
| 005 | AT-IRC                   |
| 006 | AT-IVA-SA                |
| 007 | AT-IVA-DP                |
| 008 | AT-PI                    |
| 009 | AT-IVA-Enquadramento     |
| 010 | NameNif                  |
| 011 | CE                       |
| 012 | CPP                      |
| 013 | Caderneta Predial        |
| 014 | Debt                     |
| 015 | IRSByUserPassword        |
| 016 | IRSByCode                |
| 017 | SS-DocToPay              |
| 018 | SS-No-Debt               |
| 019 | SS-SA                    |
| 020 | Vehicles-by-Nif          |
| 021 | Responsabilidade-Credito |
| 022 | Estado-Empresa           |
| 023 | NifName                  |
| 024 | Seguro-by-matricula      |
| 025 | IES                      |
| 026 | CPRC                     |

## bizAPIs Standard Codes

| Status Code | Message Code                                                              |
| :---------- | :------------------------------------------------------------------------ |
| 001         | Failed to login - Website Timeout                                         |
| 002         | Failed to login - Invalid Credentials                                     |
| 003         | Failed to login - Problem reaching the authentication page                |
| 004         | Failed to login; Failed to authenticate                                   |
| 005         | Missing authentication parameters                                         |
| 006         | The input nif is incorrect; Invalid NIF; NIF is not valid, NIPC not found |
| 007         | Problem processing the request                                            |
| 008         | Problem loading the page (timeout)                                        |
| 009         | RSM not available                                                         |
| 010         | Unable to access resource site                                            |
| 011         | Fail to obtain a response                                                 |

<br />

| Status Code | Message Code                                                      |
| :---------- | :---------------------------------------------------------------- |
| 102         | Certificate code not found                                        |
| 103         | Document doesn't exist                                            |
| 104         | No results found                                                  |
| 105         | No vehicles registered                                            |
| 106         | No data found for the license plate                               |
| 107         | Error reading file                                                |
| 108         | No companies found with the name                                  |
| 109         | Problem extracting the document for request id:                   |
| 201         | Error solving captcha                                             |
| 202         | Failed to extract document,  Failed to extract data               |
| 203         | Error searching for document                                      |
| 206         | Page not found. Negative numbers are not allowed. Page limit is 2 |
| 207         | Something went wrong encoding the file for b64                    |
| 208         | Driver had some problems initing...                               |
| 209         | Awaiting decision                                                 |