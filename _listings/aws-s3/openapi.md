swagger: "2.0"
x-collection-name: AWS S3
x-complete: 1
info:
  title: No Title
  version: 1.0.0
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