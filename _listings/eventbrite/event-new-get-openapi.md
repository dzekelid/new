---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Event New
  description: This method creates a new event. It returns the ID of the newly created
    event.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /event_new:
    get:
      summary: Get Event New
      description: This method creates a new event. It returns the ID of the newly
        created event.
      operationId: Get_event_new_
      x-api-path-slug: event-new-get
      parameters:
      - in: query
        name: background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_border_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: capacity
        description: The maximum number of people who can attend the event
      - in: query
        name: currency
        description: The event currency in ISO 4217 format (e
      - in: query
        name: custom_footer
        description: Custom HTML footer for your registration page
      - in: query
        name: custom_header
        description: Custom HTML header for your registration page
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The event description
      - in: query
        name: end_date
        description: The event end date and time, in ISO 8601 format (e
      - in: query
        name: organizer_id
        description: The event organizer ID
      - in: query
        name: personalized_url
        description: The event registration URL
      - in: query
        name: privacy
        description: 0 for a private event, 1 for a public event
      - in: query
        name: start_date
        description: The event start date and time, in ISO 8601 format (e
      - in: query
        name: status
        description: The event status
      - in: query
        name: text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: timezone
        description: The event time zone in relation to GMT (e
      - in: query
        name: title
        description: The event title
      - in: query
        name: title_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: venue_id
        description: The event venue ID
      responses:
        200:
          description: OK
      tags:
      - Event
      - New
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