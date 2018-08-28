{
  "info": {
    "name": "GIGANDCROWD Get Notify Messages",
    "_postman_id": "da689fcb-9a84-4c73-8b73-333e4815556f",
    "description": "Get notify messages.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Notify",
      "item": [
        {
          "id": "99340915-573b-44d6-bd39-81961e15863b",
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
              "id": "56ab2621-a9df-4426-8e54-681c3c0264ab"
            }
          ]
        }
      ]
    }
  ]
}