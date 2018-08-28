{
  "info": {
    "name": "Data.gov API Get Notifications",
    "_postman_id": "73983c3f-5475-4d5f-8e33-ba22cc215042",
    "description": "List all current user pending notifications",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "notifications",
      "item": [
        {
          "id": "5e875ba4-50cc-4b42-8c67-df790ea0353d",
          "name": "getNotifications",
          "request": {
            "url": "http://catalog.data.gov/api/3/notifications/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all current user pending notifications"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acef2fc3-a6d9-476f-b3b2-3c90829197e9"
            }
          ]
        }
      ]
    }
  ]
}