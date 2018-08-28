---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 GET Bucket notification
  version: 1.0.0
  description: This implementation of the GET operation uses thenotification subresource
    to return the notificationconfiguration of a bucket
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?notification:
    get:
      summary: GET Bucket notification
      description: This implementation of the GET operation uses thenotification subresource
        to return the notificationconfiguration of a bucket
      operationId: get-bucket-notification
      x-api-path-slug: notification-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Notification
    put:
      summary: PUT Bucket notification
      description: The Amazon S3 notification feature enables you to receive notifications
        when certain eventshappen in your bucket
      operationId: put-bucket-notification
      x-api-path-slug: notification-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Notification
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