# API SPEC

## CREATE PRODUCT
- Method: POST
- ENDPOINT: 'api/products'
- Header:
    - Content-Type: application/json
    - Accept: application/json
- Body: 

```json
{
  "id" : "string, unique",
  "name" : "string",
  "price" : "long",
  "quantity" : "integer",
  "createAt" : "date"
}

```

- Response:

```json
{
  "code" : "number",
  "status" : "string",
  "data" : {
    "id" : "string, unique",
    "name" : "string",
    "price" : "long",
    "quantity" : "integer",
    "createAt" : "date"
  }
}

```

## GET PRODUCT

- Method: GET
- ENDPOINT: 'api/products/{id_product}'
- Header:
    - Accept: application/json
- Response: 
```json
{
  "code" : "number",
  "status" : "string",
  "data" : {
    "id" : "string, unique",
    "name" : "string",
    "price" : "long",
    "quantity" : "integer",
    "createAt" : "date"
  }
}

```

## UPDATE PRODUCT

- Method: PATCH || PUT
- ENDPOINT: 'api/products/{id_products}'
- Header:
  - Content-Type: application/json
  - Accept: application/json
- Body:

```json
{
  "name" : "string",
  "price" : "long",
  "quantity" : "integer",
  "createAt" : "date",
  "updateAt" : "date"
}

```

- Response:

```json
{
  "code" : "number",
  "status" : "string",
  "data" : {
    "id" : "string, unique",
    "name" : "string",
    "price" : "long",
    "quantity" : "integer",
    "createAt" : "date"
  }
}

```

## LIST PRODUCT

- Method: GET
- ENDPOINT: 'api/products'
- Header:
  - Accept: application/json
- Querry Param : 
  - Size: number,
  - Page: number

- Response:

```json
{
  "code" : "number",
  "status" : "string",
  "data" : [
    {
      "id" : "string, unique",
      "name" : "string",
      "price" : "long",
      "quantity" : "integer",
      "createAt" : "date"
    },
    {
      "id" : "string, unique",
      "name" : "string",
      "price" : "long",
      "quantity" : "integer",
      "createAt" : "date"
    }
  ]
}
```

## DELETE PRODUCT

- Method: DELETE
- ENDPOINT: 'api/products/{id_products}'
- Header:
  - Accept: application/json

- Response:

```json
{
  "code" : "number",
  "status" : "string"
  }
}
```


