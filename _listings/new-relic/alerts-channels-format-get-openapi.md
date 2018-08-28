---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Alerts Channels. Format
  version: 1.0.0
  description: |-
    This API endpoint works with new Alerts on alerts.newrelic.com.

    It returns a list of the channels associated with your New Relic account.

    See our documentation for a discussion on listing notification channels.
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