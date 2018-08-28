swagger: "2.0"
x-collection-name: Vinli
x-complete: 1
info:
  title: Vinli
  description: todo-add-description
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /notifications/E4A2E663-D23B-4398-8B91-B826D5477B8F:
    get:
      summary: Get a Specific Notification
      description: Get a specific notification.
      operationId: NotificationsE4A2E663D23B43988B91B826D5477B8FGet
      x-api-path-slug: notificationse4a2e663d23b43988b91b826d5477b8f-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Notification
  /subscriptions/78acd627-e2ea-4b34-9599-b94b2f10f2f9/notifications:
    get:
      summary: Get Notifications for a Subscription
      description: Get notifications for a subscription.
      operationId: Subscriptions78acd627E2ea4b349599B94b2f10f2f9NotificationsGet
      x-api-path-slug: subscriptions78acd627e2ea4b349599b94b2f10f2f9notifications-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Notificationsa
      - Subscription
  /events/d69cc8be-a809-441d-8a70-1bf0a0d48fb3/notifications:
    get:
      summary: Get Notifications for an Event
      description: Get notifications for an event.
      operationId: EventsD69cc8beA809441d8a701bf0a0d48fb3NotificationsGet
      x-api-path-slug: eventsd69cc8bea809441d8a701bf0a0d48fb3notifications-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Notificationsan
      - Event