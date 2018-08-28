---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Intelligent Mapping Add a new collection
  description: |-
    Add a new collection of data in the form of a GeoJSON FeatureCollection.
    All coordinates must be in EPSG:4326 (WGS84) (for further details see
    http://epsg.io/4326). Any feature that is not compliant with the GeoJSON
    specification will not be stored. Any feature that doesn't contain an id
    will not be stored. If the specified collection already exists, the
    geospatial data will be appended to the existing data. Features with matching
    id's are overwritten.
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /
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