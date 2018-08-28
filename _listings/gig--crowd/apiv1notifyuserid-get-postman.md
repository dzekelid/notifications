{
  "info": {
    "name": "GIGANDCROWD Get Notify Userid",
    "_postman_id": "6d14aa59-238a-4b14-aa4d-2e74a2ba1d8e",
    "description": "Get notify userid.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Notify",
      "item": [
        {
          "id": "01b57f68-123b-4426-99b5-d7ba23dce852",
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
              "id": "163cbb89-4ffb-42f4-af7d-d68235a8796d"
            }
          ]
        },
        {
          "id": "e86981c1-c82e-4d36-8153-f3d62c796e91",
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
              "id": "8a52d4e8-d668-4b94-ab11-745aad0a39b2"
            }
          ]
        },
        {
          "id": "345dd1bc-91aa-473a-ba39-b7af17ba5fe8",
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
              "id": "5f372d1c-893a-478f-b316-e1789b9b93a5"
            }
          ]
        },
        {
          "id": "2b3e4018-32a6-48ee-80ef-28569e69f296",
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
              "id": "d30d97b1-54da-4c75-94ac-4d0d2f59f5f5"
            }
          ]
        },
        {
          "id": "c433e278-1050-4ff5-ad7a-7bf058390081",
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
              "id": "5ec6586f-a918-4d99-bec2-ad0795663e38"
            }
          ]
        },
        {
          "id": "3e523a9b-9851-4de1-999c-04d23158cfbb",
          "name": "getApiV1NotifyMessages",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/notify/messages",
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
            "description": "Get notify messages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f29aba88-6367-4e73-bd53-680b9c3ec4f3"
            }
          ]
        },
        {
          "id": "38b0c2d2-c6b5-4e48-9b1d-317f6305679e",
          "name": "getApiV1NotifyUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/notify/:userId"
              ],
              "variable": [
                {
                  "id": "userId",
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
            "description": "Get notify userid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84ac1bb1-72d2-42d1-97c5-2f337561adb3"
            }
          ]
        }
      ]
    }
  ]
}