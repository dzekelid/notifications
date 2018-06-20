---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 1
info:
  title: PagerDuty
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /notifications:
    get:
      summary: List notifications
      description: List notifications for a given time range, optionally filtered
        by type (sms_notification, email_notification, phone_notification, or push_notification).
      operationId: list-notifications-for-a-given-time-range-optionally-filtered-by-type-sms-notification-email-notific
      x-api-path-slug: notifications-get
      parameters:
      - in: query
        name: filter
        description: Return notification of this type only
      - in: query
        name: include[]
        description: Array of additional details to include
      - in: query
        name: No Name
      - in: query
        name: since
        description: The start of the date range over which you want to search
      - in: query
        name: until
        description: The end of the date range over which you want to search
      responses:
        200:
          description: OK
      tags:
      - Notifications
---