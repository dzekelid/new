---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Creates new assignment.
  description: Creates new assignment.
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/vexp/roadside/assignments:
    post:
      summary: Creates new assignment.
      description: Creates new assignment.
      operationId: postServiceVexpRoadsideAssignments
      x-api-path-slug: servicevexproadsideassignments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - CreateAssistance
      - new
      - assignment.
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