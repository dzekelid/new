---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Create a new metafield for a product.
  description: Create a new metafield for a product..
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/custom_collections.json:
    post:
      summary: Create a new custom collection
      description: Create a new custom collection.
      operationId: postAdminCustomCollections.json
      x-api-path-slug: admincustom-collections-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Custom
      - Collection
  /admin/blogs/62581763/articles.json:
    post:
      summary: Create a new article for a blog
      description: Create a new article for a blog.
      operationId: postAdminBlogs62581763Articles.json
      x-api-path-slug: adminblogs62581763articles-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Articlea
      - Blog
  /admin/metafields.json:
    post:
      summary: Create a new metafield for a store.
      description: Create a new metafield for a store..
      operationId: postAdminMetafields.json
      x-api-path-slug: adminmetafields-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Metafielda
      - Store
  /admin/blogs.json:
    post:
      summary: Create a new blog
      description: Create a new blog.
      operationId: postAdminBlogs.json
      x-api-path-slug: adminblogs-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Blog
  /admin/application_charges.json:
    post:
      summary: Create a new one-time application charge.
      description: Create a new one-time application charge..
      operationId: postAdminApplicationCharges.json
      x-api-path-slug: adminapplication-charges-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - One-time
      - Application
      - Charge
  //admin/comments.json:
    post:
      summary: Create a new comment for an article
      description: Create a new comment for an article.
      operationId: postAdminComments.json
      x-api-path-slug: admincomments-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Commentan
      - Article
  /admin/customers/3989659651/addresses.json:
    post:
      summary: Creating a new address for a customer
      description: Creating a new address for a customer.
      operationId: postAdminCustomers3989659651Addresses.json
      x-api-path-slug: admincustomers3989659651addresses-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Creating
      - New
      - Addressa
      - Customer
  /admin/gift_cards.json:
    post:
      summary: Create a new gift card with an automatically generated code
      description: Create a new gift card with an automatically generated code.
      operationId: postAdminGiftCards.json
      x-api-path-slug: admingift-cards-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Gift
      - Card
      - Automatically
      - Generated
      - Code
  /admin/orders/4554953422/refunds.json:
    post:
      summary: Create a new refund for an order
      description: Create a new refund for an order.
      operationId: postAdminOrders4554953422Refunds.json
      x-api-path-slug: adminorders4554953422refunds-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Refundan
      - Order
  /admin/smart_collections.json:
    post:
      summary: Create a new collection
      description: Create a new collection.
      operationId: postAdminSmartCollections.json
      x-api-path-slug: adminsmart-collections-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Collection
  /admin/products/7990943555/images.json:
    post:
      summary: Create a new product image
      description: Create a new product image.
      operationId: postAdminProducts7990943555Images.json
      x-api-path-slug: adminproducts7990943555images-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Product
      - Image
  /admin/customers/3989659651/addresses/5436816654/default.json:
    put:
      summary: assigning a new default address to a customer
      description: Assigning a new default address to a customer.
      operationId: putAdminCustomers3989659651Addresses5436816654Default.json
      x-api-path-slug: admincustomers3989659651addresses5436816654default-json-put
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Assigning
      - New
      - Default
      - Address
      - To
      - Customer
  /admin/pages.json:
    post:
      summary: Create a new page
      description: Create a new page.
      operationId: postAdminPages.json
      x-api-path-slug: adminpages-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Page
  /admin/products/7990943555/variants.json:
    post:
      summary: Create a new product variant
      description: Create a new product variant.
      operationId: postAdminProducts7990943555Variants.json
      x-api-path-slug: adminproducts7990943555variants-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Product
      - Variant
  /admin/customer_saved_searches.json:
    post:
      summary: Create a new Customer Saved Search
      description: Create a new customer saved search.
      operationId: postAdminCustomerSavedSearches.json
      x-api-path-slug: admincustomer-saved-searches-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Customer
      - Saved
      - Search
  /admin/redirects.json:
    post:
      summary: Create a new redirect.
      description: Create a new redirect..
      operationId: postAdminRedirects.json
      x-api-path-slug: adminredirects-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Redirect
  /admin/script_tags.json:
    post:
      summary: create a new script tag
      description: Create a new script tag.
      operationId: postAdminScriptTags.json
      x-api-path-slug: adminscript-tags-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Create
      - New
      - Script
      - Tag
  /admin/products/7990943555/metafields.json:
    post:
      summary: Create a new metafield for a product.
      description: Create a new metafield for a product..
      operationId: postAdminProducts7990943555Metafields.json
      x-api-path-slug: adminproducts7990943555metafields-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Metafielda
      - Product
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