{
  "info": {
    "name": "SendGrid Get Partner Settings New Relic",
    "_postman_id": "98c84764-a5e4-4aca-aac8-00150c6d461d",
    "description": "**This endpoint allows you to retrieve your current New Relic partner settings.**\n\nOur partner settings allow you to integrate your SendGrid account with our partners to increase your SendGrid experience and functionality. For more information about our partners, and how you can begin integrating with them, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/partners.html).\n\nBy integrating with New Relic, you can send your SendGrid email statistics to your New Relic Dashboard. If you enable this setting, your stats will be sent to New Relic every 5 minutes. You will need your New Relic License Key to enable this setting. For more information, please see our [Classroom](https://sendgrid.com/docs/Classroom/Track/Collecting_Data/new_relic.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "93929d3f-aa4d-4cb2-8bcd-66e5d6a51962",
          "name": "partner_settings.new_relic.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/partner_settings/new_relic",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current New Relic partner settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52182723-fabc-4948-b386-8dec7f9f92c9"
            }
          ]
        }
      ]
    }
  ]
}