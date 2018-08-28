---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Applications. Format
  version: 1.0.0
  description: "This API endpoint returns a paginated\nlist of the Applications associated
    with your New Relic account. The time range for summary data is the last 10 minutes.\n\nApplications
    can be filtered by their name, hosts, the list of application IDs or the application
    language as\nreported by the agents.\n\nSee our documentation for a discussion
    and examples of\nusing  filters \nand summary data output."
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts_channels.{format}:
    get:
      summary: Get Alerts Channels. Format
      description: |-
        This API endpoint works with new Alerts on alerts.newrelic.com.

        It returns a list of the channels associated with your New Relic account.

        See our documentation for a discussion on listing notification channels.
      operationId: getAlertsChannels.Format
      x-api-path-slug: alerts-channels-format-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Channels.
      - Format
    post:
      summary: Add Alerts Channels. Format
      description: "This API endpoint works with new Alerts on alerts.newrelic.com.\n\nIt
        creates a channel associated with your New Relic account.\n\nNote: Admin User???s
        API Key is required.\n\nSee our documentation for a discussion on creating
        notification channels.\n\nChannel type configuration options:\n\n\n  \n    Email\n\n
        \   {\n\n    \"recipients\" : \"test@google.com\",\n\"include_json_attachment\"
        : true\n\n\n    }\n  \n  \n    HipChat\n\n    {\n\n    \"auth_token\": \"abc123\",\n\"room_id\":
        \"google.com\"\n\n\n    }\n  \n  \n    OpsGenie\n\n    {\n\n    \"api_key\":
        \"abc123\",\n\"teams\": \"team1\",\n\"tags\": \"tag1\",\n\"recipients\": \"me@me.com\"\n\n\n
        \   }\n  \n  \n    Slack\n\n    {\n\n    \"url\": \"http://test.com\",\n\"channel\":
        \"channel1\"\n\n\n    }\n  \n  \n    Campfire\n\n    {\n\n    \"subdomain\":
        \"mysubdomain\",\n\"token\": \"123abc\",\n\"room\": \"room1\"\n\n\n    }\n
        \ \n  \n    Victorops\n\n    {\n\n    \"key\": \"mykey\",\n\"route_key\":
        \"theroute\"\n\n\n    }\n  \n  \n    PagerDuty\n\n    {\n\n    \"service_key\":
        \"myservicekey\"\n\n\n    }\n  \n  \n    Webhook (json)\n\n    {\n\n    \"base_url\":
        \"http://test.com\",\n\"auth_username\": \"username\",\n\"auth_password\":
        \"password\",\n\"payload_type\": \"application/json\",\n\"payload\": {\"account_id\":
        1, \"account_name\": \"account name\" },\n\"headers\": {\"header1\": \"test\",
        \"header2\": \"test\"}\n\n\n    }\n  \n  \n    Webhook (x-www-form-urlencoded)\n\n
        \   {\n\n    \"base_url\": \"http://test.com\",\n\"auth_username\": \"username\",\n\"auth_password\":
        \"password\",\n\"payload_type\": \"application/x-www-form-urlencoded\",\n\"payload\":
        {\"account_id\": 1, \"account_name\": \"account name\" },\n\"headers\": {\"header1\":
        \"test\", \"header2\": \"test\"}\n\n\n    }"
      operationId: postAlertsChannels.Format
      x-api-path-slug: alerts-channels-format-post
      parameters:
      - in: body
        name: channel
        description: channel schema
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: policy_ids
        description: Policy IDs to associate with channel
        type: array
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Channels.
      - Format
  /alerts_incidents.{format}:
    get:
      summary: Get Alerts Incents. Format
      description: "This API endpoint returns a list of the Incidents associated with
        your New Relic account.\n\nSee our documentation for a discussion on listing
        incidents \nand output pagination."
      operationId: getAlertsIncents.Format
      x-api-path-slug: alerts-incidents-format-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Incents.
      - Format
  /alerts_violations.{format}:
    get:
      summary: Get Alerts Violations. Format
      description: "This API endpoint works with new Alerts on alerts.newrelic.com.\n\nIt
        returns a list of the violations associated with your New Relic account.\n\nSee
        our documentation for a discussion on \noutput pagination."
      operationId: getAlertsViolations.Format
      x-api-path-slug: alerts-violations-format-get
      parameters:
      - in: query
        name: only_open
        description: Filter by open violations
        type: boolean
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Violations.
      - Format
  /applications.{format}:
    get:
      summary: Get Applications. Format
      description: "This API endpoint returns a paginated\nlist of the Applications
        associated with your New Relic account. The time range for summary data is
        the last 10 minutes.\n\nApplications can be filtered by their name, hosts,
        the list of application IDs or the application language as\nreported by the
        agents.\n\nSee our documentation for a discussion and examples of\nusing  filters
        \nand summary data output."
      operationId: getApplications.Format
      x-api-path-slug: applications-format-get
      parameters:
      - in: query
        name: filter[host]
        description: Filter by application host
        type: string
      - in: query
        name: filter[ids]
        description: Filter by application ids
        type: list
      - in: query
        name: filter[language]
        description: Filter by application language
        type: string
      - in: query
        name: filter[name]
        description: Filter by application name
        type: string
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications.
      - Format
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