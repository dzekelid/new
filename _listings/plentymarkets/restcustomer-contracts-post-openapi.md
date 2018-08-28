---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Creates a new contract
  description: Creates a new contract.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
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
  /rest/boards:
    post:
      summary: Creates a new board.
      description: Creates a new board..
      operationId: postRestBoards
      x-api-path-slug: restboards-post
      parameters:
      - in: body
        name: /rest/boards
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Board
  /rest/boards/{boardId}/columns:
    post:
      summary: Creates a new column and assigns it to a given board
      description: Creates a new column and assigns it to a given board.
      operationId: postRestBoardsBoardColumns
      x-api-path-slug: restboardsboardidcolumns-post
      parameters:
      - in: body
        name: /rest/boards/{boardId}/columns
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Column
      - Assigns
      - It
      - To
      - Given
      - Board
  /rest/boards/{boardId}/columns/{columnId}/tasks:
    post:
      summary: Creates a new tasks on a specified column.
      description: Creates a new tasks on a specified column..
      operationId: postRestBoardsBoardColumnsColumnTasks
      x-api-path-slug: restboardsboardidcolumnscolumnidtasks-post
      parameters:
      - in: body
        name: /rest/boards/{boardId}/columns/{columnId}/tasks
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: boardId
      - in: path
        name: columnId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Tasks
      - "On"
      - Specified
      - Column
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}/references:
    post:
      summary: Creates a new reference from a given task to a contact or a ticket.
      description: Creates a new reference from a given task to a contact or a ticket..
      operationId: postRestBoardsBoardColumnsColumnTasksTaskReferences
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskidreferences-post
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: referenceValue
        description: Reference type followed by foreign ID of the referenced object
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Reference
      - From
      - Given
      - Task
      - To
      - Contact
      - Ticket
  /rest/categories:
    post:
      summary: Creates new categories
      description: Creates new categories.
      operationId: postRestCategories
      x-api-path-slug: restcategories-post
      parameters:
      - in: body
        name: /rest/categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Categories
  /rest/customer_contracts:
    post:
      summary: Creates a new contract
      description: Creates a new contract.
      operationId: postRestCustomerContracts
      x-api-path-slug: restcustomer-contracts-post
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Contract
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