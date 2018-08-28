---
swagger: "2.0"
x-collection-name: Quovo
x-complete: 0
info:
  title: Quovo Create a new access token
  description: Creates and returns a new Access Token.
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