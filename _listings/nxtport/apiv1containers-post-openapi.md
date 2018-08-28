---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: NxtPort T-mining Secure Container Release API Create a new Container
  description: |-
    Create a new container.
    If all goes well, a 200 status code is returned.
    If the create fails, a 500 status code is returned.
  contact:
    name: T-Mining API support
    url: http://support.t-mining.be/
    email: support@t-mining.be
  version: 1.0.0
host: api.nxtport.eu
basePath: /blockchain
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/containers:
    post:
      summary: Create a new Container
      description: |-
        Create a new container.
        If all goes well, a 200 status code is returned.
        If the create fails, a 500 status code is returned.
      operationId: postApiV1Containers
      x-api-path-slug: apiv1containers-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Container
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