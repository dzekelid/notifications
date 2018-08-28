{
  "info": {
    "name": "GIGANDCROWD Get Notify Requests",
    "_postman_id": "75d73807-93b2-4850-b22b-ad3abc0d12c6",
    "description": "Get notify requests.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Notify",
      "item": [
        {
          "id": "a3a5108c-03da-45db-ad3e-9909b6bd02ba",
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
              "id": "9911512b-2e4a-4768-9c85-33d4eecf6f6f"
            }
          ]
        },
        {
          "id": "6969755f-e3d4-4b47-a0da-3e8065dc7f81",
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
              "id": "a046a6f1-f6cd-4fad-9448-6537092fc269"
            }
          ]
        },
        {
          "id": "f70066ca-fa16-4082-83d2-f591d2e5555d",
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
              "id": "37df02e2-3f3d-4106-aecc-455c07da53ca"
            }
          ]
        },
        {
          "id": "138c2376-d929-418d-a325-7b0513f368db",
          "name": "getApiV1NotifyArtistsNew",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/notify/artists/new",
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
            "description": "Get notify artists new."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2237784-bfe5-4465-968a-b38575ad63f8"
            }
          ]
        },
        {
          "id": "978a4d6c-66de-46c8-8644-6052d1df5ca9",
          "name": "getApiV1NotifyRequests",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/notify/requests",
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
            "description": "Get notify requests."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38d529e0-6238-4da4-b933-42dd714ad2bd"
            }
          ]
        }
      ]
    }
  ]
}