---
name: Predix
x-slug: predix
description: Predix (IoT PaaS) helps you develop apps that connect people with industrial
  machines through analytics and data for better business outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
x-kinRank: "7"
x-alexaRank: "264121"
tags: New
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/predix/apis.md
specificationVersion: "0.14"
apis:
- name: Intelligent Mapping - Add a new collection
  x-api-slug: v1collectionscollectionname-post
  description: |-
    Add a new collection of data in the form of a GeoJSON FeatureCollection.
    All coordinates must be in EPSG:4326 (WGS84) (for further details see
    http://epsg.io/4326). Any feature that is not compliant with the GeoJSON
    specification will not be stored. If the specified collection already
    exists, the geospatial data will be appended to the existing data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/predix/v1collectionscollectionname-post-openapi.md
- name: Intelligent Mapping - Add a new collection
  x-api-slug: v1collectionscollectionname-put
  description: |-
    Add a new collection of data in the form of a GeoJSON FeatureCollection.
    All coordinates must be in EPSG:4326 (WGS84) (for further details see
    http://epsg.io/4326). Any feature that is not compliant with the GeoJSON
    specification will not be stored. Any feature that doesn't contain an id
    will not be stored. If the specified collection already exists, the
    geospatial data will be appended to the existing data. Features with matching
    id's are overwritten.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/predix/v1collectionscollectionname-put-openapi.md
- name: Intelligent Mapping - Create a new layer
  x-api-slug: v1mapsmapidlayers-post
  description: Creates a new layer and associates it with the specified map.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/predix/v1mapsmapidlayers-post-openapi.md
- name: VIEWS - Creates a new instance in tags of this Tag.
  x-api-slug: decksidtags-post
  description: Creates a new instance in tags of this tag..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////v1
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/predix/decksidtags-post-openapi.md
- name: VIEWS - Create a new instance of the Deck and persist it.
  x-api-slug: decks-post
  description: Create a new instance of the deck and persist it..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////v1
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/predix/decks-post-openapi.md
- name: VIEWS - Creates a new instance in tags of this Card.
  x-api-slug: cardsidtags-post
  description: Creates a new instance in tags of this card..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////v1
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/predix/cardsidtags-post-openapi.md
- name: VIEWS - Create a new instance of the Cards and persist it.
  x-api-slug: cards-post
  description: Create a new instance of the cards and persist it..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////v1
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/predix/cards-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://predicthq.api.gallery.streamdata.io
- type: x-api-stack
  url: http://predix.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/predix
- type: x-documentation
  url: https://docs.predix.io/en-US/platform
- type: x-twitter
  url: https://twitter.com/Predix
- type: x-website
  url: https://www.predix.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---