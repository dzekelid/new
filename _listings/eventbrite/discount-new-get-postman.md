{
  "info": {
    "name": "Eventbrite Get Discount New",
    "_postman_id": "881cb0a3-0771-46a7-8c0d-8bb8e456180e",
    "description": "This method creates a new discount code for a specific event. It returns the ID of the newly created discount code.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Checkout",
      "item": [
        {
          "id": "09840355-a330-40db-ad98-12c561417b9e",
          "name": "getCheckoutSettingsCountriesCurrencies",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/checkout_settings/countries_currencies/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the countries and currencies which are supported by Eventbrite for ticket payment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d80c4e2-dbd7-401d-bd71-975329b158ba"
            }
          ]
        }
      ]
    },
    {
      "name": "Discounts",
      "item": [
        {
          "id": "91924ad8-0026-4037-bd5b-84dd7a193537",
          "name": "getDiscountsDiscount",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/:discount_id/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the cross_event_discount with the specified :discount_id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c7160ef-f250-45a1-87f6-96f0e4ae10a6"
            }
          ]
        },
        {
          "id": "affea084-851f-4c57-8d1a-41163e92d70f",
          "name": "postDiscountsDiscount",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/:discount_id/?discount.amount_off=%7B%7D&discount.code=%7B%7D&discount.end_date=%7B%7D&discount.end_date_relative=%7B%7D&discount.hold_ids=%7B%7D&discount.percent_off=%7B%7D&discount.quantity_available=%7B%7D&discount.start_date=%7B%7D&discount.start_date_relative=%7B%7D&discount.ticket_class_ids=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the discount with the specified :discount_id. Returns the updated cross_event_discount. The fields sent are the ones that are going to be updated, the fields that are not sent will be unchanged. The same conditions and notes for the discount creation apply."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf13924b-4fa3-4e58-8147-2d6196a68ee6"
            }
          ]
        },
        {
          "id": "a7ab081e-82aa-4035-b85e-b1f5d059a5c3",
          "name": "deleteDiscountsDiscount",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/:discount_id/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the cross_event_discount with the specified :discount_id.\nOnly unused discounts can be deleted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9217fa7-76b2-4b4b-b5b5-5398a6d562cb"
            }
          ]
        },
        {
          "id": "776de022-e877-4b2b-8a0a-cd2e85a31550",
          "name": "postDiscounts",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/?discount.amount_off=%7B%7D&discount.code=%7B%7D&discount.end_date=%7B%7D&discount.end_date_relative=%7B%7D&discount.event_id=%7B%7D&discount.hold_ids=%7B%7D&discount.percent_off=%7B%7D&discount.quantity_available=%7B%7D&discount.start_date=%7B%7D&discount.start_date_relative=%7B%7D&discount.ticket_class_ids=%7B%7D&discount.ticket_group_id=%7B%7D&discount.type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a discount. Returns the created cross_event_discount."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74ed9750-294f-4487-86a7-48b9637c0b0a"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "775b5a84-c78a-4505-806d-21251f307dae",
          "name": "getEventsDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aae85738-7a9b-4342-9476-3e7ff2b21612"
            }
          ]
        },
        {
          "id": "51413a6f-367c-46aa-9d85-8b7176da03c4",
          "name": "postEventsDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5752ba18-d4ff-42e5-b5db-65c48713f9bd"
            }
          ]
        },
        {
          "id": "f8d523da-6255-4859-8a15-328a030cd6f5",
          "name": "getEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ddf65706-02ca-48f4-b7d1-0c5d3bd3e98e"
            }
          ]
        },
        {
          "id": "ad1de8cd-bec0-4a40-abe8-c9edac247745",
          "name": "postEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ddc517cd-84b7-45e0-9d2a-1526752743e6"
            }
          ]
        },
        {
          "id": "e8f0c0d5-18e6-4bdf-aca6-9e0f5dd229c2",
          "name": "deleteEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f513b39c-ee59-4550-aaf8-944eddc0b55b"
            }
          ]
        },
        {
          "id": "dd20662c-ab02-4b26-9d14-923acf7e14a7",
          "name": "getEventsPublicDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "340cef98-5296-461c-98c8-89e1a9d92152"
            }
          ]
        },
        {
          "id": "9369d8d9-6eab-49d5-82a9-e9baeb966e5d",
          "name": "postEventsPublicDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2902e41-a840-4d59-8bf7-4e11fe1d48d1"
            }
          ]
        },
        {
          "id": "2ba02405-97f8-42d7-8977-aebc136f4e77",
          "name": "getEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b570638f-98fd-4abf-9b23-f82d0611b3a7"
            }
          ]
        },
        {
          "id": "7b68c5c1-453b-415b-b52c-77d24cc5b03a",
          "name": "postEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b63b720a-274d-45a4-8987-baa1db60bf58"
            }
          ]
        },
        {
          "id": "0580b430-2ea0-4634-a4d8-b0a1356ddab3",
          "name": "deleteEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0a1ba0e-2380-470d-8287-ef11674b742d"
            }
          ]
        }
      ]
    },
    {
      "name": "System",
      "item": [
        {
          "id": "162e5e64-8f5f-4029-9380-4e3adbade903",
          "name": "getSystemCountries",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/system/countries/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single page response with a key of countries,\ncontaining a list of countries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "056cb2c5-8ae8-4e3f-ad87-d1f778e6043f"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "3d60b0be-757f-4706-96ff-a1aac4fdb67c",
          "name": "getUsersUserDiscounts",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/users/:user_id/discounts/?code=%7B%7D&code_filter=%7B%7D&event_id=%7B%7D&order_by=%7B%7D&page_size=%7B%7D&scope=%7B%7D&ticket_group_id=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated response of cross_event_discount for the specified user.\nThis operation is only supported for the currently authenticated user. The alias me (/users/me/) may be used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8c55269-975a-476c-9bdd-bcac6985952a"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "dc699cc6-b411-45f4-ad6f-9444d4864f83",
          "name": "Get_event_list_discounts_",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/event_list_discounts?data-type=%7B%7D&id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method returns a list of discounts for a given event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42b93358-b5ad-4efe-b85b-5b06fde9f277"
            }
          ]
        }
      ]
    },
    {
      "name": "Discount",
      "item": [
        {
          "id": "b6371fc2-b5fd-45fa-8990-0a377e481b75",
          "name": "Get_discount_new_",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discount_new?amount_off=%7B%7D&code=%7B%7D&data-type=%7B%7D&end_date=%7B%7D&event_id=%7B%7D&percent_off=%7B%7D&quantity_available=%7B%7D&start_date=%7B%7D&tickets=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method creates a new discount code for a specific event. It returns the ID of the newly created discount code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1b8fd67-f664-4bd8-a8e5-d74b1fc93914"
            }
          ]
        }
      ]
    }
  ]
}