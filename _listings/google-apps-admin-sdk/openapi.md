swagger: "2.0"
x-collection-name: Google Apps Admin SDK
x-complete: 1
info:
  title: Google Apps Admin SDK Merged API
  version: 1.0.0
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