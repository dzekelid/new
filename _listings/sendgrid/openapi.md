swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /partner_settings/new_relic:
    get:
      summary: Get Partner Settings New Relic
      description: |-
        **This endpoint allows you to retrieve your current New Relic partner settings.**

        Our partner settings allow you to integrate your SendGrid account with our partners to increase your SendGrid experience and functionality. For more information about our partners, and how you can begin integrating with them, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/partners.html).

        By integrating with New Relic, you can send your SendGrid email statistics to your New Relic Dashboard. If you enable this setting, your stats will be sent to New Relic every 5 minutes. You will need your New Relic License Key to enable this setting. For more information, please see our [Classroom](https://sendgrid.com/docs/Classroom/Track/Collecting_Data/new_relic.html).
      operationId: partner_settings.new_relic.get
      x-api-path-slug: partner-settingsnew-relic-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Partner
      - Settings
      - New
      - Relic
    patch:
      summary: Patch Partner Settings New Relic
      description: |-
        **This endpoint allows you to update or change your New Relic partner settings.**

        Our partner settings allow you to integrate your SendGrid account with our partners to increase your SendGrid experience and functionality. For more information about our partners, and how you can begin integrating with them, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/partners.html).

        By integrating with New Relic, you can send your SendGrid email statistics to your New Relic Dashboard. If you enable this setting, your stats will be sent to New Relic every 5 minutes. You will need your New Relic License Key to enable this setting. For more information, please see our [Classroom](https://sendgrid.com/docs/Classroom/Track/Collecting_Data/new_relic.html).
      operationId: partner_settings.new_relic.patch
      x-api-path-slug: partner-settingsnew-relic-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Partner
      - Settings
      - New
      - Relic