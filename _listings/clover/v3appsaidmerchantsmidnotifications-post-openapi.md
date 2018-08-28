---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Create a notification for an app
  version: 1.0.0
  description: 'Push a message to all merchant devices that have your app installed
    and are listening for notifications.  For details on how to use Clover''s Android
    SDK to receive notifications see: https://github.com/clover/android-examples/tree/master/pushnotificationexample'
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/apps/{aId}/merchants/{mId}/notifications:
    post:
      summary: Create a notification for an app
      description: 'Push a message to all merchant devices that have your app installed
        and are listening for notifications.  For details on how to use Clover''s
        Android SDK to receive notifications see: https://github.com/clover/android-examples/tree/master/pushnotificationexample'
      operationId: CreateMerchantAppNotification
      x-api-path-slug: v3appsaidmerchantsmidnotifications-post
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Merchants
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