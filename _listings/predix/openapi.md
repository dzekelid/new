---
swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /decks/{id}/tags:
    post:
      summary: Creates a new instance in tags of this Tag.
      description: Creates a new instance in tags of this tag..
      operationId: postDecksTags
      x-api-path-slug: decksidtags-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Instance
      - In
      - Tags
      - Of
      - This
      - Tag
  /decks:
    post:
      summary: Create a new instance of the Deck and persist it.
      description: Create a new instance of the deck and persist it..
      operationId: postDecks
      x-api-path-slug: decks-post
      parameters:
      - in: body
        name: data
        description: Deck instance data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Instance
      - Of
      - Deck
      - Persist
      - It
  /cards/{id}/tags:
    post:
      summary: Creates a new instance in tags of this Card.
      description: Creates a new instance in tags of this card..
      operationId: postCardsTags
      x-api-path-slug: cardsidtags-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Instance
      - In
      - Tags
      - Of
      - This
      - Card
  /cards:
    post:
      summary: Create a new instance of the Cards and persist it.
      description: Create a new instance of the cards and persist it..
      operationId: postCards
      x-api-path-slug: cards-post
      parameters:
      - in: body
        name: data
        description: Card instance data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Instance
      - Of
      - Cards
      - Persist
      - It
---