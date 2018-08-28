{
  "info": {
    "name": "Azure Notification Hubs API Notification Hubs List Authorization Rules",
    "_postman_id": "8c20d5ee-356f-4e63-8a77-cb5ddecc4b4c",
    "description": "Gets the authorization rules for a NotificationHub.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "notification hubs authorization rules",
      "item": [
        {
          "id": "7b8e57a4-0a6a-4fef-8c6c-4c40f8eef3c2",
          "name": "NotificationHubs_ListAuthorizationRules",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.NotificationHubs/namespaces/:namespaceName/notificationHubs/:notificationHubName/AuthorizationRules"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "namespaceName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "notificationHubName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the authorization rules for a NotificationHub"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "851fd884-4165-4c78-bc95-bf907582fee9"
            }
          ]
        }
      ]
    }
  ]
}