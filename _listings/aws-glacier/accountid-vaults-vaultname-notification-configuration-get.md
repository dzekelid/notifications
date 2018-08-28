---
swagger: "2.0"
info:
  title: Amazon Glacier API Get  Vault  Notifications
  version: 1.0.0
  description: "DescriptionThis operation retrieves the notification-configuration
    subresource set on the\n\t\t\tvault (see Set Vault Notification Configuration
    (PUT\n\t\tnotification-configuration). If notification configuration for a\n\t\t\tvault
    is not set, the operation returns a 404 Not Found error. For more\n\t\t\tinformation
    about vault notifications, see Configuring Vault Notifications in Amazon Glacier.
    RequestsTo retrieve the notification configuration information, send a GET request
    to\n\t\t\tthe URI of a vault's notification-configuration subresource."
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{AccountId}/vaults/{VaultName}/notification-configuration:
    get:
      summary: Get  Vault  Notifications
      description: "DescriptionThis operation retrieves the notification-configuration
        subresource set on the\n\t\t\tvault (see Set Vault Notification Configuration
        (PUT\n\t\tnotification-configuration)"
      operationId: "Get Vault Notifications (GET\n\t\tnotification-configuration)"
      parameters:
      - in: query
        name: Events
        description: "A list of one or more events for which Amazon Glacier will send
          a notification to the\t\t\t\t\t\t\t\tspecified Amazon SNS topic"
        type: string
      - in: query
        name: SNSTopic
        description: The Amazon Simple Notification Service (Amazon SNS) topic Amazon
          Resource Name (ARN)
        type: string
      responses:
        200:
          description: OK
      tags:
      - vault notifications
definitions: []
x-collection-name: AWS Glacier
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---