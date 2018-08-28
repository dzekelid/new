swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /forms:
    post:
      summary: Create a new form
      description: Create a new form
      operationId: create-a-new-form
      x-api-path-slug: forms-post
      parameters:
      - in: formData
        name: active
        description: Form activity status
      - in: formData
        name: active_date_from
        description: If activity status is 1, this field is required
      - in: formData
        name: active_date_to
        description: If activity status is 1, this field is required
      - in: formData
        name: active_days
        description: If activity status is 4, this field is required
      - in: formData
        name: group_id
        description: The ID of the group in which you want to create the form
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: The name of the new form
      responses:
        200:
          description: OK
      tags:
      - New
      - Form
  /groups:
    post:
      summary: Create a new group
      description: Create a new group
      operationId: create-a-new-group
      x-api-path-slug: groups-post
      parameters:
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: Form name
      - in: formData
        name: parent_id
        description: Indicates the ID of the parent group
      - in: formData
        name: webhook_url
        description: The URL of the WebHook
      responses:
        200:
          description: OK
      tags:
      - New
      - Group
  /users:
    post:
      summary: Create a new subuser
      description: Create a new subuser
      operationId: create-a-new-subuser
      x-api-path-slug: users-post
      parameters:
      - in: formData
        name: admin
        description: Indicates if the subuser is admin or not
      - in: formData
        name: allow_create_form
        description: Allow or restrict subuser access to creating new forms
      - in: formData
        name: allow_delete_form
        description: Allow subusers to delete forms
      - in: formData
        name: allow_duplicate_form
        description: Allow subusers to duplicate forms
      - in: formData
        name: can_manage_groups
        description: Allow admin subusers to manage groups
      - in: formData
        name: can_manage_users
        description: Allow admin subusers to manage users
      - in: formData
        name: company_name
        description: The name of the company to which the subuser belongs
      - in: formData
        name: email
        description: Email address of the account
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: Username of the account
      - in: formData
        name: passhash
        description: MD5 password
      - in: formData
        name: password
        description: Plain text password
      responses:
        200:
          description: OK
      tags:
      - New
      - Subuser
  /accounts:
    post:
      summary: Create new account
      description: Creates a new account (standalone user). This is available only
        upon request.
      operationId: creates-a-new-account-standalone-user-this-is-available-only-upon-request
      x-api-path-slug: accounts-post
      parameters:
      - in: formData
        name: company_name
        description: The company name associated with the account
      - in: formData
        name: email
        description: The email address associated with the account
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: The username associated with the account
      - in: formData
        name: password
        description: The password associated with the account
      - in: formData
        name: password_repeat
        description: Password repeat
      - in: formData
        name: plan
        description: 'The service plan of the account: 0 - Free (default value), 1
          - Gold, 2 - Platinum, 3 - Diamond'
      responses:
        200:
          description: OK
      tags:
      - New
      - Account