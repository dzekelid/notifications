---
swagger: "2.0"
x-collection-name: AWS WorkDocs
x-complete: 1
info:
  title: AWS WorkDocs API
  version: 1.0.0
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
  /?Action=DescribeNotificationSubscriptions:
    get:
      summary: Describe Notification Subscriptions
      description: Lists the specified notification subscriptions.
      operationId: describeNotificationSubscriptions
      x-api-path-slug: actiondescribenotificationsubscriptions-get
      parameters:
      - in: query
        name: Limit
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: OrganizationId
        description: The ID of the organization
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
---