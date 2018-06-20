---
swagger: "2.0"
x-collection-name: AWS WorkDocs
x-complete: 0
info:
  title: AWS WorkDocs API Delete Notification Subscription
  version: 1.0.0
  description: Deletes the specified subscription from the specified organization.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateNotificationSubscription:
    get:
      summary: Create Notification Subscription
      description: Configure WorkDocs to use Amazon SNS notifications.
      operationId: createNotificationSubscription
      x-api-path-slug: actioncreatenotificationsubscription-get
      parameters:
      - in: query
        name: OrganizationId
        description: The ID of the organization
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /?Action=DeleteNotificationSubscription:
    get:
      summary: Delete Notification Subscription
      description: Deletes the specified subscription from the specified organization.
      operationId: deleteNotificationSubscription
      x-api-path-slug: actiondeletenotificationsubscription-get
      parameters:
      - in: query
        name: OrganizationId
        description: The ID of the organization
        type: string
      - in: query
        name: SubscriptionId
        description: The ID of the subscription
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
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