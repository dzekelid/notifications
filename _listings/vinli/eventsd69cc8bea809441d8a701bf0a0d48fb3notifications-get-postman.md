{
  "info": {
    "name": "Vinli Get Notifications for an Event",
    "_postman_id": "cd9fad87-8001-42ef-b3eb-48230ed4516b",
    "description": "Get notifications for an event.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Eventsa",
      "item": [
        {
          "id": "2c953850-c637-4356-8694-9e0742abed1d",
          "name": "Devices62976d30B6dc40f18422Ccc367572101EventsGet",
          "request": {
            "url": "http://events.vin.li/api/v1/devices/62976d30-b6dc-40f1-8422-ccc367572101/events",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all events for a device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db05d01b-178b-4d94-938a-f396f71d740a"
            }
          ]
        }
      ]
    },
    {
      "name": "Specific",
      "item": [
        {
          "id": "68f30f55-80a3-44cb-ba8a-f586c240666e",
          "name": "Events1caa8fffC9be4506Bcb838371c25aa14Get",
          "request": {
            "url": "http://events.vin.li/api/v1/events/1caa8fff-c9be-4506-bcb8-38371c25aa14",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a specific event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15699ef5-6f23-47c8-a000-ce7bbe8c446d"
            }
          ]
        }
      ]
    },
    {
      "name": "Notificationsan",
      "item": [
        {
          "id": "e69d42e8-aa59-42be-892c-b7c51728ec0a",
          "name": "EventsD69cc8beA809441d8a701bf0a0d48fb3NotificationsGet",
          "request": {
            "url": "http://events.vin.li/api/v1/events/d69cc8be-a809-441d-8a70-1bf0a0d48fb3/notifications",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get notifications for an event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35afd6df-95e1-4b3d-86a8-fc2a3f248fbf"
            }
          ]
        }
      ]
    }
  ]
}