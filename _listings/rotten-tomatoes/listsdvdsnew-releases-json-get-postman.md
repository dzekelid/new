{
  "info": {
    "name": "Rotten Tomatoes Get Lists Dvds New Releases",
    "_postman_id": "6fe9eba0-f465-48c7-aea7-42b34211a6c4",
    "description": "Get lists dvds new releases.json.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "c2a7828f-3500-4dfe-9a59-d66291da6634",
          "name": "getLists.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "609c5e1d-244f-4420-ba2c-595724b42cea"
            }
          ]
        },
        {
          "id": "69df1b25-1b86-40cf-94cb-87e49cdc5565",
          "name": "getListsDvds.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d06825b-9d23-46ad-8fb4-f11432f63dd3"
            }
          ]
        },
        {
          "id": "5b8e4061-a2b8-4df0-babc-aff0bca499c8",
          "name": "getListsDvdsCurrentReleases.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds/current_releases.json?country=%7B%7D&page=%7B%7D&page_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds current releases.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8efe8b7-b488-44bb-accd-8996c3e3d391"
            }
          ]
        },
        {
          "id": "bf2920ce-101b-4a4b-9927-f0f5761521d0",
          "name": "getListsDvdsNewReleases.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds/new_releases.json?country=%7B%7D&page=%7B%7D&page_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds new releases.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98a8a9ef-9085-4403-9fbb-6222fc606461"
            }
          ]
        }
      ]
    }
  ]
}