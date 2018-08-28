---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart Adds a new serial to the system
  version: 1.0.0
  description: Adds a new serial to the system.
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Cart:
    post:
      summary: Adds a new cart to the system
      description: Adds a new cart to the system.
      operationId: Carts_Post
      x-api-path-slug: 3dcartwebapiv1cart-post
      parameters:
      - in: body
        name: cart
        description: A Json or XML object containing the new cart
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Cart
      - To
      - System
  /3dCartWebAPI/v1/Cart/{orderkey}/Item:
    post:
      summary: Adds a new item to a cart
      description: Adds a new item to a cart.
      operationId: Carts_Post
      x-api-path-slug: 3dcartwebapiv1cartorderkeyitem-post
      parameters:
      - in: body
        name: item
        description: A Json or XML object containing the new cart item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Item
      - To
      - Cart
  /3dCartWebAPI/v1/Categories:
    post:
      summary: Adds a new category to the system
      description: Adds a new category to the system.
      operationId: Category_Post
      x-api-path-slug: 3dcartwebapiv1categories-post
      parameters:
      - in: body
        name: category
        description: A Json or XML object containing the new category
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Category
      - To
      - System
  /3dCartWebAPI/v1/Categories/{categoryid}/Options:
    post:
      summary: Adds a new OptionSet to the system
      description: Adds a new optionset to the system.
      operationId: Category_Post
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-post
      parameters:
      - in: path
        name: categoryid
        description: Category ID
      - in: body
        name: optionset
        description: A Json or XML object containing the new optionset
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - OptionSet
      - To
      - System
  /3dCartWebAPI/v1/CRM:
    post:
      summary: Adds a new CRM to the system
      description: Adds a new crm to the system.
      operationId: CRM_PostCRM
      x-api-path-slug: 3dcartwebapiv1crm-post
      parameters:
      - in: body
        name: crm
        description: A Json or XML object containing the new CRM
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - CRM
      - To
      - System
  /3dCartWebAPI/v1/CRM/{id}/message:
    post:
      summary: Adds a new CRM Message to the system
      description: Adds a new crm message to the system.
      operationId: CRM_PostMessage
      x-api-path-slug: 3dcartwebapiv1crmidmessage-post
      parameters:
      - in: path
        name: id
        description: Id of the CRM where the message will be added
      - in: body
        name: message
        description: A Json or XML object containing the new CRM message
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - CRM
      - Message
      - To
      - System
  /3dCartWebAPI/v1/CRM/savedreply:
    post:
      summary: Adds a new CRM SaveReply to the system
      description: Adds a new crm savereply to the system.
      operationId: CRM_PostSavedReply
      x-api-path-slug: 3dcartwebapiv1crmsavedreply-post
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: savereply
        description: A Json or XML object containing the new CRM SavedReply
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - CRM
      - SaveReply
      - To
      - System
  /3dCartWebAPI/v1/CustomerGroups:
    post:
      summary: Adds a new customer group to the system
      description: Adds a new customer group to the system.
      operationId: CustomerGroups_Post
      x-api-path-slug: 3dcartwebapiv1customergroups-post
      parameters:
      - in: body
        name: customergroup
        description: A Json or XML object containing the new customer group
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Customer
      - Group
      - To
      - System
  /3dCartWebAPI/v1/Customers:
    post:
      summary: Adds a new customer to the system
      description: Adds a new customer to the system.
      operationId: Customers_Post
      x-api-path-slug: 3dcartwebapiv1customers-post
      parameters:
      - in: body
        name: customer
        description: A Json or XML object containing the new customer
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Customer
      - To
      - System
  /3dCartWebAPI/v1/Distributors:
    post:
      summary: Adds a new distributor to the system
      description: Adds a new distributor to the system.
      operationId: Distributors_Post
      x-api-path-slug: 3dcartwebapiv1distributors-post
      parameters:
      - in: body
        name: distributor
        description: A Json or XML object containing the new distributor
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Distributor
      - To
      - System
  /3dCartWebAPI/v1/Manufacturers:
    post:
      summary: Adds a new manufacturer to the system
      description: Adds a new manufacturer to the system.
      operationId: Manufacturer_Post
      x-api-path-slug: 3dcartwebapiv1manufacturers-post
      parameters:
      - in: body
        name: manufacturer
        description: A Json or XML object containing the new manufacturer
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Manufacturer
      - To
      - System
  /3dCartWebAPI/v1/Orders:
    post:
      summary: Adds a new order to the system
      description: Adds a new order to the system.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1orders-post
      parameters:
      - in: query
        name: bypassorderemail
        description: will bypass sending the customer new order email if normally
          applicable
      - in: query
        name: bypassorderprocessing
        description: will bypass/ignore stock updates, gift certificates generation,
          rewards, etc
      - in: body
        name: order
        description: A Json or XML object containing the new order
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Order
      - To
      - System
  /3dCartWebAPI/v1/Orders/{orderid}/Items:
    post:
      summary: Adds a new item on the order
      description: Adds a new item on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderiditems-post
      parameters:
      - in: body
        name: item
        description: A Json or XML object containing the new item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Item
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Questions:
    post:
      summary: Adds a new question on the order
      description: Adds a new question on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestions-post
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: question
        description: A Json or XML object containing the new question
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Question
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Shipments:
    post:
      summary: Adds a new shipment on the order
      description: Adds a new shipment on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderidshipments-post
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: shipment
        description: A Json or XML object containing the new shipment
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Shipment
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Transactions:
    post:
      summary: Adds a new transaction on the order
      description: Adds a new transaction on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactions-post
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: transaction
        description: A Json or XML object containing the new transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Transaction
      - "On"
      - Order
  /3dCartWebAPI/v1/PaymentTokens:
    post:
      summary: Adds a new paymenttoken to the system
      description: Adds a new paymenttoken to the system.
      operationId: PaymentToken_Post
      x-api-path-slug: 3dcartwebapiv1paymenttokens-post
      parameters:
      - in: body
        name: paymenttoken
        description: A Json or XML object containing the new manufacturer
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Paymenttoken
      - To
      - System
  /3dCartWebAPI/v1/Products:
    post:
      summary: Adds a new product to the system
      description: Adds a new product to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1products-post
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: product
        description: A Json or XML object containing the new product
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Product
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Discount:
    post:
      summary: Adds a new discount to the system
      description: Adds a new discount to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogiddiscount-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: discount
        description: A Json or XML object containing the new discount
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Discount
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/EProducts:
    post:
      summary: Adds a new eproduct to the system
      description: Adds a new eproduct to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogideproducts-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: eproduct
        description: A Json or XML object containing the new eproduct
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Eproduct
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Features:
    post:
      summary: Adds a new feature to the system
      description: Adds a new feature to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidfeatures-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: feature
        description: A Json or XML object containing the new feature
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Feature
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Images:
    post:
      summary: Adds a new image to the system
      description: Adds a new image to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidimages-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: image
        description: A Json or XML object containing the new image
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Image
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Options:
    post:
      summary: Adds a new OptionSet to the system
      description: Adds a new optionset to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidoptions-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: optionset
        description: A Json or XML object containing the new optionset
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - OptionSet
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Related:
    post:
      summary: Adds a new related product to the system
      description: Adds a new related product to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidrelated-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: relatedproduct
        description: A Json or XML object containing the new related product
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Related
      - Product
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Serials:
    post:
      summary: Adds a new serial to the system
      description: Adds a new serial to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidserials-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: serial
        description: A Json or XML object containing the new serial
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Serial
      - To
      - System
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---