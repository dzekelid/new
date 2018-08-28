---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Notify Artists New
  version: 1.0.0
  description: Get notify artists new.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/managers/combine/{oldid}/{newid}:
    post:
      summary: Post Managers Combine Old New
      description: Post managers combine old new.
      operationId: postApiV1ManagersCombineOldNew
      x-api-path-slug: apiv1managerscombineoldidnewid-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: newid
      - in: path
        name: oldid
      responses:
        200:
          description: OK
      tags:
      - Managers
      - Combine
      - Old
      - New
  /api/v1/message/new/{withUserId}/{lastMessageId}:
    get:
      summary: Get Message New Withuserid Lastmessageid
      description: Get message new withuserid lastmessageid.
      operationId: getApiV1MessageNewWithuserLastmessage
      x-api-path-slug: apiv1messagenewwithuseridlastmessageid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: lastMessageId
      - in: path
        name: withUserId
      responses:
        200:
          description: OK
      tags:
      - Message
      - New
      - Withuserid
      - Lastmessageid
  /api/v1/notify/artists/new:
    get:
      summary: Get Notify Artists New
      description: Get notify artists new.
      operationId: getApiV1NotifyArtistsNew
      x-api-path-slug: apiv1notifyartistsnew-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Notify
      - Artists
      - New
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