{
  "info": {
    "name": "GIGANDCROWD Post Managers Combine Old New",
    "_postman_id": "76063173-74a1-4928-a4b5-5bb9bf21b2db",
    "description": "Post managers combine old new.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Managers",
      "item": [
        {
          "id": "28ddf39f-0cb1-4cd1-b262-85706b7c4401",
          "name": "postApiV1ManagersCombineOldNew",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/managers/combine/:oldid/:newid"
              ],
              "variable": [
                {
                  "id": "newid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "oldid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Post managers combine old new."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17d3ec13-09cb-428c-9ca5-3a71a539de71"
            }
          ]
        }
      ]
    }
  ]
}