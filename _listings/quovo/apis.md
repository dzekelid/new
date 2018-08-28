---
name: Quovo
x-slug: quovo
description: Quovo&rsquo;s API provides methods for retrieving data from financial
  institutions on behalf of clients, advisors, and other users. This documentation
  includes detailed explanations of API endpoints and common data definitions. Please
  note that this documentation does not list all API endpoints. Additionally, you
  may not have access to all of the listed endpoints depending on the services you&rsquo;ve
  purchased from Quovo.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
x-kinRank: "7"
x-alexaRank: "391003"
tags: New
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/quovo/apis.md
specificationVersion: "0.14"
apis:
- name: Quovo API v3 - Create a new access token
  x-api-slug: tokens-post
  description: Creates and returns a new Access Token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/quovo/tokens-post-openapi.md
- name: Quovo API v3 - Create a new Quovo User
  x-api-slug: users-post
  description: |-
    Creates a new Quovo User.

    Users are owners of Accounts, Portfolios, and any related financial data such as Positions and History.

    If you have a Postman Environment set up, the previous request should have set your Access Token automatically. If not, be sure that your Access Token is included in the current request:

    1. Click on the "Headers" tab.
    2. Enter `Authorization` as the header field.
    3. Enter `Bearer token` as the header value, where `token` should be replaced with your actual Access Token.

    After sending the request, the Environment variable `user_id` will be automatically set to the newly created User's id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/quovo/users-post-openapi.md
- name: Quovo API v3 - Request a new institution
  x-api-slug: usersuser-idinstitution-requests-post
  description: Requests a new financial institution for Quovo to retrieve data from.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/quovo/usersuser-idinstitution-requests-post-openapi.md
- name: Quovo API v3 - Register a new webhook
  x-api-slug: webhooks-post
  description: Used to register new webhooks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/quovo/webhooks-post-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.quovo.com/fintech-blog/feed/
- type: x-postman-collection
  url: https://www.getpostman.com/collections/82cf673bb22d4f8b8881
- type: x-website
  url: http://quovo.com
- type: x-api-gallery
  url: http://quandl.api.gallery.streamdata.io
- type: x-api-stack
  url: http://quovo.stack.network
- type: x-authentication
  url: https://api.quovo.com/docs/v3/#authentication
- type: x-blog
  url: https://www.quovo.com/fintech-blog/
- type: x-crunchbase
  url: https://crunchbase.com/organization/quovo
- type: x-developer
  url: https://api.quovo.com/docs/v3/
- type: x-email
  url: audit@quovo.com
- type: x-email
  url: info@quovo.com
- type: x-email
  url: copyright@quovo.com
- type: x-email
  url: support@quovo.com
- type: x-github
  url: https://github.com/quovo
- type: x-twitter
  url: https://twitter.com/quovo
- type: x-webhook
  url: https://api.quovo.com/docs/v3/#webhooks
- type: x-website
  url: https://www.quovo.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---