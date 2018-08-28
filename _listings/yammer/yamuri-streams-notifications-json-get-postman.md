{
  "info": {
    "name": "Yammer API Get Notifications",
    "_postman_id": "eb35f7b9-c105-4c6f-bfbb-da75e4d68a2f",
    "description": "Get the notifications feed for the current user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "notifications",
      "item": [
        {
          "id": "86fca62c-184c-446c-bc37-bb96a7d38579",
          "name": "Get_Notifications_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/streams/notifications.json"
              ],
              "variable": [
                {
                  "id": "yamURI",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the notifications feed for the current user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d80894c-7e53-4146-9747-f953e03a017f"
            }
          ]
        }
      ]
    }
  ]
}