swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/collections/{collectionName}:
    post:
      summary: Add a new collection
      description: |-
        Add a new collection of data in the form of a GeoJSON FeatureCollection.
        All coordinates must be in EPSG:4326 (WGS84) (for further details see
        http://epsg.io/4326). Any feature that is not compliant with the GeoJSON
        specification will not be stored. If the specified collection already
        exists, the geospatial data will be appended to the existing data.
      operationId: add-a-new-collection-of-data-in-the-form-of-a-geojson-featurecollectionall-coordinates-must-be-in-ep
      x-api-path-slug: v1collectionscollectionname-post
      parameters:
      - in: body
        name: body
        description: Geospatial data for the collection
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Collection
    put:
      summary: Add a new collection
      description: |-
        Add a new collection of data in the form of a GeoJSON FeatureCollection.
        All coordinates must be in EPSG:4326 (WGS84) (for further details see
        http://epsg.io/4326). Any feature that is not compliant with the GeoJSON
        specification will not be stored. Any feature that doesn't contain an id
        will not be stored. If the specified collection already exists, the
        geospatial data will be appended to the existing data. Features with matching
        id's are overwritten.
      operationId: add-a-new-collection-of-data-in-the-form-of-a-geojson-featurecollectionall-coordinates-must-be-in-ep
      x-api-path-slug: v1collectionscollectionname-put
      parameters:
      - in: body
        name: body
        description: Geospatial data for the collection
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Collection
  /v1/maps/{mapId}/layers:
    post:
      summary: Create a new layer
      description: Creates a new layer and associates it with the specified map.
      operationId: creates-a-new-layer-and-associates-it-with-the-specified-map
      x-api-path-slug: v1mapsmapidlayers-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Layer
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