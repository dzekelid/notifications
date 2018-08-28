{
  "info": {
    "name": "Azure Notification Hubs API Notification Hubs Delete Authorization Rule",
    "_postman_id": "596dcb0a-dddf-4f2b-8a31-12a2fb4d002f",
    "description": "Deletes a notificationHub authorization rule",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "notification hubs authorization rule",
      "item": [
        {
          "id": "f0b45d07-2c87-40a7-b824-4b43827c3c26",
          "name": "NotificationHubs_DeleteAuthorizationRule",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.NotificationHubs/namespaces/:namespaceName/notificationHubs/:notificationHubName/AuthorizationRules/:authorizationRuleName"
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
                  "id": "authorizationRuleName",
                  "value": "{}",
                  "type": "string"
                },
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a notificationHub authorization rule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a05302b5-bc53-45e0-8e30-029cf5588a26"
            }
          ]
        }
      ]
    }
  ]
}