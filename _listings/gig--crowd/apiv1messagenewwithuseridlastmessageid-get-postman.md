{
  "info": {
    "name": "GIGANDCROWD Get Message New Withuserid Lastmessageid",
    "_postman_id": "f1707b7a-4555-4033-a4d5-d0c2e22389e0",
    "description": "Get message new withuserid lastmessageid.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Managers",
      "item": [
        {
          "id": "cf8a661e-87de-4ca5-9bac-c64285cc8bf1",
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
              "id": "04dcb2a9-c4f3-491b-94a6-fb66dc5c7d9d"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "dd1c4674-1e04-4692-a162-bf0401b22b2c",
          "name": "getApiV1MessageNewWithuserLastmessage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/message/new/:withUserId/:lastMessageId"
              ],
              "variable": [
                {
                  "id": "lastMessageId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "withUserId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
            "description": "Get message new withuserid lastmessageid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d69e178-7c2c-438b-91e7-9ed39b6cf38a"
            }
          ]
        }
      ]
    }
  ]
}