---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Notification Channels  . Format
  version: 1.0.0
  description: |-
    WARNING: This is legacy alerting.  This endpoint will be deprecated.

    This API endpoint returns a single notification channel, identified by ID.???
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /notification_channels.{format}:
    get:
      summary: Get Notification Channels. Format
      description: "WARNING: This is legacy alerting.  This endpoint will be deprecated.\n\nThis
        API endpoint returns a paginated \nlist of the notification channels associated
        with your New Relic account.\n\nNotification channels can be filtered by their
        type or a list of IDs."
      operationId: getNotificationChannels.Format
      x-api-path-slug: notification-channels-format-get
      parameters:
      - in: query
        name: filter[ids]
        description: Filter by notification channel IDs
        type: list
      - in: query
        name: filter[type]
        description: Filter by notification channel types
        type: list
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Channels.
      - Format
  /notification_channels/{id}.{format}:
    get:
      summary: Get Notification Channels  . Format
      description: |-
        WARNING: This is legacy alerting.  This endpoint will be deprecated.

        This API endpoint returns a single notification channel, identified by ID.???
      operationId: getNotificationChannels.Format
      x-api-path-slug: notification-channelsid-format-get
      parameters:
      - in: path
        name: id
        description: Notification Channel ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Channels
      - ""
      - .
      - Format
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