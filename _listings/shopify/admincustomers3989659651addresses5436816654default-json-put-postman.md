{
  "info": {
    "name": "Shopify assigning a new default address to a customer",
    "_postman_id": "0be38c1b-6888-464c-8fe4-1c10ae07fc11",
    "description": "Assigning a new default address to a customer.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "a3be00b7-9df2-48a6-8563-cdf2ffc2b758",
          "name": "getAdminCustomers3989659651Addresses.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/3989659651/addresses.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
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
            "description": "Get all of a customer's addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d319064f-afec-4aca-8c4d-fc7d6180b5c6"
            }
          ]
        },
        {
          "id": "eaab88a2-fb8e-4cb4-b8e2-5b423b2f3165",
          "name": "putAdminCustomers3989659651AddressesSet.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/3989659651/addresses/set.json?address_ids=%5B%7B%7D%5D&operation=%7B%7D",
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
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
            "description": "Destroying multiple customer addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcaf3cfb-3647-4da8-9759-a96cdc6614c8"
            }
          ]
        },
        {
          "id": "7769827b-9e21-4621-b7ff-2385c55c3816",
          "name": "deleteAdminCustomers3989659651Addresses5484465742.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/3989659651/addresses/5484465742.json",
            "method": "DELETE",
            "header": [
              {
                "key": "Content-Type",
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
            "description": "Removing a customers address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53c12b7a-6a02-4230-9581-493516e5d2f4"
            }
          ]
        },
        {
          "id": "e621d0bb-6418-4db3-b517-77bf5fb03524",
          "name": "getAdminCustomersSearch.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/search.json?query=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
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
            "description": "Get all customers with an address in the brazil."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a1bbfc0-183f-4c3b-abfc-21583bbab3d5"
            }
          ]
        },
        {
          "id": "ab1d450a-c3e7-44b4-a717-0167391ecbb7",
          "name": "putAdminCustomers3989659651Addresses5436816654Default.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/3989659651/addresses/5436816654/default.json",
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
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
            "description": "Assigning a new default address to a customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51aa49db-af35-4544-979f-cd8e12546d84"
            }
          ]
        }
      ]
    }
  ]
}