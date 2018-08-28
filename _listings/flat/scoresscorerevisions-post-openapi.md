---
swagger: "2.0"
x-collection-name: Flat
x-complete: 0
info:
  title: Flat Create a new revision
  description: Update a score by uploading a new revision for this one.
  termsOfService: https://flat.io/legal
  contact:
    name: Flat
    url: https://flat.io/support
    email: developers@flat.io
  version: 2.1.0
host: api.flat.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /scores:
    post:
      summary: Create a new score
      description: |-
        Use this API method to **create a new music score in the current User account**. You will need a MusicXML 3 (`vnd.recordare.musicxml` or `vnd.recordare.musicxml+xml`) or a MIDI (`audio/midi`) file to create the new Flat document.

        This API call will automatically create the first revision of the document, the score can be modified by the using our web application or by uploading a new revision of this file (`POST /v2/scores/{score}/revisions/{revision}`).

        The currently authenticated user will be granted owner of the file and will be able to add other collaborators (users and groups).
      operationId: createScore
      x-api-path-slug: scores-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Score
  /scores/{score}/collaborators:
    post:
      summary: Add a new collaborator
      description: |-
        Share a score with a single user or a group. This API call allows to add, invite and update the collaborators of a document.
        - To add an existing Flat user to the document, specify its unique identifier in the `user` property.
        - To invite an external user to the document, specify its email in the `userEmail` property.
        - To add a Flat group to the document, specify its unique identifier in the `group` property.
        - To update an existing collaborator, process the same request with different rights.
      operationId: addScoreCollaborator
      x-api-path-slug: scoresscorecollaborators-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Collaborator
  /scores/{score}/comments:
    post:
      summary: Post a new comment
      description: |-
        Post a document or a contextualized comment on a document.

        Please note that this method includes an anti-spam system for public scores. We don't guarantee that your comments will be accepted and displayed to end-user. Comments are be blocked by returning a `403` HTTP error and hidden from other users when the `spam` property is `true`.
      operationId: postScoreComment
      x-api-path-slug: scoresscorecomments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Comment
  /scores/{score}/revisions:
    post:
      summary: Create a new revision
      description: Update a score by uploading a new revision for this one.
      operationId: createScoreRevision
      x-api-path-slug: scoresscorerevisions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Revision
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