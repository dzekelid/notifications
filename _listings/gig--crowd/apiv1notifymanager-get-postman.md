{
  "info": {
    "name": "GIGANDCROWD Get Notify Manager",
    "_postman_id": "aa33f993-a367-4c9c-a742-99f259e6f313",
    "description": "Get notify manager.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Notify",
      "item": [
        {
          "id": "8ac58156-e41d-47a2-b85a-c0078aa98b7d",
          "name": "getApiV1NotifyUnpayed",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/notify/unpayed",
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
            "description": "Get notify unpayed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "faa843bc-4881-452e-90cc-ce5243d886ae"
            }
          ]
        },
        {
          "id": "eff386d8-08e1-43e3-a743-1b1ab596619f",
          "name": "getApiV1NotifyArtists",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/notify/artists",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get notify artists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd4aef5f-4912-4c74-bec9-2146e0168a29"
            }
          ]
        },
        {
          "id": "8022abc6-ae1b-40d0-9b61-529f61cd36bb",
          "name": "getApiV1NotifyManager",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/notify/manager",
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
            "description": "Get notify manager."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "739a8116-a215-4f00-b30e-8cce977414d8"
            }
          ]
        }
      ]
    }
  ]
}