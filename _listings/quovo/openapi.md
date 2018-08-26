---
swagger: "2.0"
x-collection-name: Quovo
x-complete: 1
info:
  title: Quovo API v3
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tokens:
    post:
      summary: Create a new access token
      description: Creates and returns a new Access Token.
      operationId: TokensPost4
      x-api-path-slug: tokens-post
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
      - New
      - Access
      - Token
  /users:
    post:
      summary: Create a new Quovo User
      description: |-
        Creates a new Quovo User.

        Users are owners of Accounts, Portfolios, and any related financial data such as Positions and History.

        If you have a Postman Environment set up, the previous request should have set your Access Token automatically. If not, be sure that your Access Token is included in the current request:

        1. Click on the "Headers" tab.
        2. Enter `Authorization` as the header field.
        3. Enter `Bearer token` as the header value, where `token` should be replaced with your actual Access Token.

        After sending the request, the Environment variable `user_id` will be automatically set to the newly created User's id.
      operationId: UsersPost4
      x-api-path-slug: users-post
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
      - New
      - Quovo
      - User
  /users/{user_id}/institution_requests:
    post:
      summary: Request a new institution
      description: Requests a new financial institution for Quovo to retrieve data
        from.
      operationId: UsersInstitutionRequestsByUserIdPost
      x-api-path-slug: usersuser-idinstitution-requests-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Request
      - New
      - Institution
  /webhooks:
    post:
      summary: Register a new webhook
      description: Used to register new webhooks.
      operationId: WebhooksPost
      x-api-path-slug: webhooks-post
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
      - Register
      - New
      - Webhook
---