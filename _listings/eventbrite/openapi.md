---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: create-manage--promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
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
  /ticket_new:
    get:
      summary: Get Ticket New
      description: This method creates new fixed-price or donation ticket types. It
        returns the ID of the newly created ticket.
      operationId: Get_ticket_new_
      x-api-path-slug: ticket-new-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The ticket description
      - in: query
        name: end_sales
        description: The date and time when ticket sales stop, in ISO 8601 format
          (e
      - in: query
        name: event_id
        description: The event ID
      - in: query
        name: include_fee
        description: 0 to add the Eventbrite service fee on top of ticket price, or
          1 to include it in the ticket price
      - in: query
        name: is_donation
        description: 0 for fixed-price tickets, 1 for donations
      - in: query
        name: max
        description: The maximum number of tickets per order
      - in: query
        name: min
        description: The minimum number of tickets per order
      - in: query
        name: name
        description: The ticket name
      - in: query
        name: price
        description: The ticket price
      - in: query
        name: quantity
        description: The number of tickets available
      - in: query
        name: start_sales
        description: The date and time when ticket sales start, in ISO 8601 format
          (e
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - New
  /venue_new:
    get:
      summary: Get Venue New
      description: This method creates a new venue. It returns the ID of the newly
        created venue.
      operationId: Get_venue_new_
      x-api-path-slug: venue-new-get
      parameters:
      - in: query
        name: adress
        description: The venue address (line 1)
      - in: query
        name: adress_2
        description: The venue address (line 2)
      - in: query
        name: city
        description: The venue city
      - in: query
        name: country_code
        description: 2-letter country code, according to the ISO 3166 format
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: organizer_id
        description: The ID of the related organizer
      - in: query
        name: postal_code
        description: The postal code of the venue
      - in: query
        name: region
        description: The venue state/province/county/territory depending on the country
      - in: query
        name: venue
        description: The venue name
      responses:
        200:
          description: OK
      tags:
      - Venue
      - New
  /organizer_new:
    get:
      summary: Get Organizer New
      description: Many event creators prefer having a specific person identified
        as the point of contact for their event. This person is usually someone like
        the event emcee, or an on-site contact that can help with attendee check-ins
        or other issues during the event. This method creates a new organizer, and
        returns the organizer_id for the newly created resource.
      operationId: Get_organizer_new_
      x-api-path-slug: organizer-new-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The organizer description
      - in: query
        name: name
        description: The organizer name
      responses:
        200:
          description: OK
      tags:
      - Organizer
      - New
  /user_new:
    get:
      summary: Get User New
      description: This method creates a new user, returning the user???s ID in the
        response.
      operationId: Get_user_new_
      x-api-path-slug: user-new-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: email
        description: The user email address
      - in: query
        name: passwd
        description: The user password
      responses:
        200:
          description: OK
      tags:
      - User
      - New
  /discount_new:
    get:
      summary: Get Discount New
      description: This method creates a new discount code for a specific event. It
        returns the ID of the newly created discount code.
      operationId: Get_discount_new_
      x-api-path-slug: discount-new-get
      parameters:
      - in: query
        name: amount_off
        description: The fixed amount off the ticket price
      - in: query
        name: code
        description: The discount code
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: end_date
        description: The discount end date and time, in ISO 8601 format (e
      - in: query
        name: event_id
        description: The event ID
      - in: query
        name: percent_off
        description: The percentage off the ticket price
      - in: query
        name: quantity_available
        description: Maximum number of times this discount can be used
      - in: query
        name: start_date
        description: The discount start date and time, in ISO 8601 format (e
      - in: query
        name: tickets
        description: Comma-separated list of ticket IDs for which the discount applies
      responses:
        200:
          description: OK
      tags:
      - Discount
      - New
---