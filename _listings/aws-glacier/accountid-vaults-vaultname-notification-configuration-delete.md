---
swagger: "2.0"
info:
  title: Amazon Glacier API Delete  Vault  Notifications
  version: 1.0.0
  description: "DescriptionThis operation deletes the notification configuration set
    for a vault \n\t\t\tSet Vault Notification Configuration (PUT\n\t\tnotification-configuration).
    The operation is\n\t\t\teventually consistent&#8212;that is, it might take some
    time for Amazon Glacier to\n\t\t\tcompletely disable the notifications, and you
    might still receive some notifications for\n\t\t\ta short time after you send
    the delete request. RequestsTo delete a vault's notification configuration, send
    a DELETE request to the\n\t\t\tvault's notification-configuration subresource."
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{AccountId}/vaults/{VaultName}/notification-configuration:
    delete:
      summary: Delete  Vault  Notifications
      description: "DescriptionThis operation deletes the notification configuration
        set for a vault \n\t\t\tSet Vault Notification Configuration (PUT\n\t\tnotification-configuration)"
      operationId: "Delete Vault Notifications (DELETE\n\t\tnotification-configuration)"
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