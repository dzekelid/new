---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
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
---