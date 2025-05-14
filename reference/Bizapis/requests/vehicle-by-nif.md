---
title: Vehicles-by-Nif
excerpt: >-
  This endpoint allows users to search details of all vehicles corresponding to
  the respective number.
api:
  file: bizapis.json
  operationId: vehicle-by-nif
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
> <h3 style={{ textAlign: "center" }}>DOWNLOAD PROJECT</h3>
> <ul>
>   <li><a href="https://we.tl/t-362cCpxLXw" target="_blank">Java</a></li>
>   <li><a href="https://we.tl/t-Su796XuSgQ">Python</a></li>
>   <li><a href="https://we.tl/t-nZotH0R6Vx">C#</a></li>
> </ul>
> `}</HTMLBlock>

<HTMLBlock>{`
<a href="https://www.bizapis.com/wp-content/uploads/2024/08/servico_vehicles_by_nif.mp4.mp4" target="_blank">To watch the video click here</a>
`}</HTMLBlock>

# JSON Schema API Response

```json PT
{  
  "type" : "object",  
  "properties" : {  
    "requestId" : {  
      "type" : "string",  
      "description" : "Identificador único do pedido."  
    },  
    "nif" : {  
      "type" : "string",  
      "description" : "Número de Identificação Fiscal (NIF)."  
    },  
    "name" : {  
      "type" : "string",  
      "description" : "Nome do proprietário ou responsável pelo veículo."  
    },  
    "licensePlate" : {  
      "type" : "string",  
      "description" : "Matrícula do veículo."  
    },  
    "licensePlateIssueDate" : {  
      "type" : "string",  
      "description" : "Data de emissão da matrícula."  
    },  
    "firstRegistrationDate" : {  
      "type" : "string",  
      "description" : "Data da primeira matrícula do veículo."  
    },  
    "brand" : {  
      "type" : "string",  
      "description" : "Marca do veículo."  
    },  
    "model" : {  
      "type" : "string",  
      "description" : "Modelo do veículo."  
    },  
    "color" : {  
      "type" : "string",  
      "description" : "Cor do veículo."  
    },  
    "category" : {  
      "type" : "string",  
      "description" : "Categoria do veículo, como definido pela autoridade competente."  
    },  
    "seatingCapacity" : {  
      "type" : "string",  
      "description" : "Capacidade de lotação do veículo (número de assentos)."  
    },  
    "vehicleType" : {  
      "type" : "string",  
      "description" : "Tipo de veículo."  
    },  
    "fuelType" : {  
      "type" : "string",  
      "description" : "Tipo de combustível utilizado pelo veículo."  
    },  
    "squareNumber" : {  
      "type" : "string",  
      "description" : "Número do quadro do veículo."  
    },  
    "cylinderCapacity" : {  
      "type" : "string",  
      "description" : "Cilindrada do motor."  
    },  
    "power" : {  
      "type" : "string",  
      "description" : "Potência do motor."  
    },  
    "voltage" : {  
      "type" : "string",  
      "description" : "Voltagem do sistema elétrico do veículo."  
    },  
    "grossWeight" : {  
      "type" : "string",  
      "description" : "Peso bruto do veículo."  
    },  
    "towableGrossWeight" : {  
      "type" : "string",  
      "description" : "Peso bruto rebocável permitido pelo veículo."  
    },  
    "co2Emission" : {  
      "type" : "string",  
      "description" : "Emissão de CO2 do veículo."  
    },  
    "co2calculationMethod" : {  
      "type" : "string",  
      "description" : "Método utilizado para calcular as emissões de CO2."  
    },  
    "wankleEngine" : {  
      "type" : "string",  
      "description" : "Indicação se o motor do veículo é do tipo Wankel."  
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
      "description": "Unique identifier for the request."
    },
    "nif": {
      "type": "string",
      "description": "Tax Identification Number (NIF)."
    },
    "name": {
      "type": "string",
      "description": "Name of the vehicle owner or responsible party."
    },
    "licensePlate": {
      "type": "string",
      "description": "Vehicle license plate."
    },
    "licensePlateIssueDate": {
      "type": "string",
      "description": "Date of issuance of the license plate."
    },
    "firstRegistrationDate": {
      "type": "string",
      "description": "Date of the vehicle's first registration."
    },
    "brand": {
      "type": "string",
      "description": "Brand of the vehicle."
    },
    "model": {
      "type": "string",
      "description": "Model of the vehicle."
    },
    "color": {
      "type": "string",
      "description": "Color of the vehicle."
    },
    "category": {
      "type": "string",
      "description": "Category of the vehicle as defined by the relevant authority."
    },
    "seatingCapacity": {
      "type": "string",
      "description": "Seating capacity of the vehicle (number of seats)."
    },
    "vehicleType": {
      "type": "string",
      "description": "Type of vehicle."
    },
    "fuelType": {
      "type": "string",
      "description": "Type of fuel used by the vehicle."
    },
    "squareNumber": {
      "type": "string",
      "description": "Frame number of the vehicle."
    },
    "cylinderCapacity": {
      "type": "string",
      "description": "Engine displacement."
    },
    "power": {
      "type": "string",
      "description": "Power of the engine."
    },
    "voltage": {
      "type": "string",
      "description": "Voltage of the vehicle's electrical system."
    },
    "grossWeight": {
      "type": "string",
      "description": "Gross weight of the vehicle."
    },
    "towableGrossWeight": {
      "type": "string",
      "description": "Maximum towable gross weight of the vehicle."
    },
    "co2Emission": {
      "type": "string",
      "description": "CO2 emission of the vehicle."
    },
    "co2calculationMethod": {
      "type": "string",
      "description": "Method used to calculate CO2 emissions."
    },
    "wankleEngine": {
      "type": "string",
      "description": "Indicates whether the vehicle's engine is of the Wankel type."
    }
  }
}
```