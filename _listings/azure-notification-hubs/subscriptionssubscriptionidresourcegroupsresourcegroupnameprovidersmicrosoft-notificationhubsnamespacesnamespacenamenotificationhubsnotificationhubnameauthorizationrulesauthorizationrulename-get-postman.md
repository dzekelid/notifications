{
  "info": {
    "name": "Azure Notification Hubs API Notification Hubs Get Authorization Rule",
    "_postman_id": "56a3454b-b4f4-4a70-b836-780c4f92a2aa",
    "description": "Gets an authorization rule for a NotificationHub by name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "notification hubs authorization rule",
      "item": [
        {
          "id": "dbc0cfb4-7c58-4428-b816-8fa676c42768",
          "name": "NotificationHubs_GetAuthorizationRule",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets an authorization rule for a NotificationHub by name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e46b69cc-068f-438c-9d0b-622c0a4c7235"
            }
          ]
        }
      ]
    }
  ]
}