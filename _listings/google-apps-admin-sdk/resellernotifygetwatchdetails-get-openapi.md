---
swagger: "2.0"
x-collection-name: Google Apps Admin SDK
x-complete: 0
info:
  title: Google Apps Admin SDK API Get Watch Details
  version: 1.0.0
  description: Returns all the details of the watch corresponding to the reseller.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /resellernotify/getwatchdetails:
    get:
      summary: Get Watch Details
      description: Returns all the details of the watch corresponding to the reseller.
      operationId: reseller.resellernotify.getwatchdetails
      x-api-path-slug: resellernotifygetwatchdetails-get
      responses:
        200:
          description: OK
      tags:
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