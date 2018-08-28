---
swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 0
info:
  title: BigCommerce Create a new category
  description: ""
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store-hash}/v3/catalog/products/{id}/images:
    post:
      summary: Upload a new product image to a single product
      description: Adds a new product image from a publicly accessible URL. May fail
        if the hosting website is forcing HTTPS connections with TLS 1.0 (as this
        has been deprecated).
      operationId: V3CatalogProductsImagesByStoreHashAndIdPost
      x-api-path-slug: storehashv3catalogproductsidimages-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Upload
      - New
      - Product
      - Image
      - To
      - Single
      - Product
  /{store-hash}/v3/catalog/products:
    post:
      summary: Create a new product with variants
      description: Sample request for creating a new product with variants through
        V3 Catalog API
      operationId: V3CatalogProductsByStoreHashPost
      x-api-path-slug: storehashv3catalogproducts-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Product
      - Variants
  /{store_hash}/v3/catalog/brands:
    post:
      summary: Create a new brand
      description: ""
      operationId: V3CatalogBrandsByStoreHashPost
      x-api-path-slug: store-hashv3catalogbrands-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Brand
  /{store_hash}/v3/customers/subscribers:
    post:
      summary: Create a new subscriber
      description: ""
      operationId: V3CustomersSubscribersByStoreHashPost
      x-api-path-slug: store-hashv3customerssubscribers-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Subscriber
  /{store_hash}/v3/catalog/categories:
    post:
      summary: Create a new category
      description: ""
      operationId: V3CatalogCategoriesByStoreHashPost
      x-api-path-slug: store-hashv3catalogcategories-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Category
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