swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
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