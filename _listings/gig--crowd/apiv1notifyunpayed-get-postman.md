{
  "info": {
    "name": "GIGANDCROWD Get Notify Unpayed",
    "_postman_id": "6b742f67-1108-4548-899a-2e8d4a4e7864",
    "description": "Get notify unpayed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Notify",
      "item": [
        {
          "id": "5b73e046-aa42-4b3d-a6a5-26e466b687d1",
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
              "id": "033f75e1-3412-4453-a81e-b4b582bc0258"
            }
          ]
        }
      ]
    }
  ]
}