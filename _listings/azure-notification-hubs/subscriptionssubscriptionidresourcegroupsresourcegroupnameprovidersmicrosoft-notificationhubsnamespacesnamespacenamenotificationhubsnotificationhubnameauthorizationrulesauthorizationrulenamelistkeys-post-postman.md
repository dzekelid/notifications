{
  "info": {
    "name": "Azure Notification Hubs API Notification Hubs List Keys",
    "_postman_id": "2be59ed8-1564-49fb-b71c-526ab486b401",
    "description": "Gets the Primary and Secondary ConnectionStrings to the NotificationHub",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "notification hubs keys",
      "item": [
        {
          "id": "10c422a8-a66f-43fe-bcc4-9889b4784aa0",
          "name": "NotificationHubs_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.NotificationHubs/namespaces/:namespaceName/notificationHubs/:notificationHubName/AuthorizationRules/:authorizationRuleName/listKeys"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the Primary and Secondary ConnectionStrings to the NotificationHub "
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14be06fd-1518-47a5-95a8-788296766263"
            }
          ]
        }
      ]
    }
  ]
}