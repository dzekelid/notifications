{
  "info": {
    "name": "Azure DevTest Labs API Notification Channels Delete",
    "_postman_id": "54ba13c0-dbb2-4e6d-9b62-c429481bad61",
    "description": "Delete notificationchannel.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "notification channels",
      "item": [
        {
          "id": "5cc62e9d-fd59-498a-80d3-b0e3eba63f98",
          "name": "NotificationChannels_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DevTestLab/labs/:labName/notificationchannels/:name"
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
                  "id": "labName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete notificationchannel"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64ad0f7e-8d3e-463a-b427-73228eff8be7"
            }
          ]
        }
      ]
    }
  ]
}