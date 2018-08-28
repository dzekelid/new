---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Generate a new token
  description: |-
    Generate a new token for the command based on command id string.
    ##### Permissions
    Must have `manage_slash_commands` permission for the team the command is in.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /jobs:
    post:
      summary: Create a new job.
      description: |-
        Create a new job.
        __Minimum server version: 4.1__
        ##### Permissions
        Must have `manage_jobs` permission.
      operationId: create-a-new-job-minimum-server-version-41--permissionsmust-have-manage-jobs-permission
      x-api-path-slug: jobs-post
      parameters:
      - in: body
        name: body
        description: Job object to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Job.
  /commands/{command_id}/regen_token:
    put:
      summary: Generate a new token
      description: |-
        Generate a new token for the command based on command id string.
        ##### Permissions
        Must have `manage_slash_commands` permission for the team the command is in.
      operationId: generate-a-new-token-for-the-command-based-on-command-id-string-permissionsmust-have-manage-slash-co
      x-api-path-slug: commandscommand-idregen-token-put
      parameters:
      - in: path
        name: command_id
        description: ID of the command to generate the new token
      responses:
        200:
          description: OK
      tags:
      - Generate
      - New
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