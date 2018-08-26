---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 1
info:
  title: HitBTC API
  description: create-api-keys-in-your-profile-httpshitbtc-comsettingsapikeys-and-use-public-api-key-as-username-and-secret-as-password-to-authorize-
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /order:
    post:
      summary: Create New Order
      description: Create new order.
      operationId: postOrder
      x-api-path-slug: order-post
      parameters:
      - in: formData
        name: clientOrderId
      - in: formData
        name: expireTime
      - in: formData
        name: price
      - in: formData
        name: quantity
      - in: formData
        name: side
      - in: formData
        name: stopPrice
      - in: formData
        name: strictValidate
        description: Strict validate amount and price precision without rounding
      - in: formData
        name: symbol
      - in: formData
        name: timeInForce
      - in: formData
        name: type
      responses:
        200:
          description: OK
      tags:
      - New
      - Order
  /order/{clientOrderId}:
    put:
      summary: Create New Order
      description: Create new order.
      operationId: putOrderClientorder
      x-api-path-slug: orderclientorderid-put
      parameters:
      - in: path
        name: clientOrderId
      - in: formData
        name: expireTime
      - in: formData
        name: price
      - in: formData
        name: quantity
      - in: formData
        name: side
      - in: formData
        name: stopPrice
      - in: formData
        name: strictValidate
        description: Strict validate amount and price precision without rounding
      - in: formData
        name: symbol
      - in: formData
        name: timeInForce
      - in: formData
        name: type
      responses:
        200:
          description: OK
      tags:
      - New
      - Order
  /account/crypto/address/{currency}:
    post:
      summary: Create New Deposit Crypro Address
      description: Create new deposit crypro address.
      operationId: postAccountCryptoAddressCurrency
      x-api-path-slug: accountcryptoaddresscurrency-post
      parameters:
      - in: path
        name: currency
      responses:
        200:
          description: OK
      tags:
      - New
      - Deposit
      - Crypro
      - Address
---