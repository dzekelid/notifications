---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Notify Userid
  version: 1.0.0
  description: Post notify userid.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/notify/unpayed:
    get:
      summary: Get Notify Unpayed
      description: Get notify unpayed.
      operationId: getApiV1NotifyUnpayed
      x-api-path-slug: apiv1notifyunpayed-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Notify
      - Unpayed
  /api/v1/notify/artists:
    get:
      summary: Get Notify Artists
      description: Get notify artists.
      operationId: getApiV1NotifyArtists
      x-api-path-slug: apiv1notifyartists-get
      responses:
        200:
          description: OK
      tags:
      - Notify
      - Artists
  /api/v1/notify/manager:
    get:
      summary: Get Notify Manager
      description: Get notify manager.
      operationId: getApiV1NotifyManager
      x-api-path-slug: apiv1notifymanager-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Notify
      - Manager
  /api/v1/notify/artists/new:
    get:
      summary: Get Notify Artists New
      description: Get notify artists new.
      operationId: getApiV1NotifyArtistsNew
      x-api-path-slug: apiv1notifyartistsnew-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Notify
      - Artists
      - New
  /api/v1/notify/requests:
    get:
      summary: Get Notify Requests
      description: Get notify requests.
      operationId: getApiV1NotifyRequests
      x-api-path-slug: apiv1notifyrequests-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Notify
      - Requests
  /api/v1/notify/messages:
    get:
      summary: Get Notify Messages
      description: Get notify messages.
      operationId: getApiV1NotifyMessages
      x-api-path-slug: apiv1notifymessages-get
      responses:
        200:
          description: OK
      tags:
      - Notify
      - Messages
  /api/v1/notify/{userId}:
    get:
      summary: Get Notify Userid
      description: Get notify userid.
      operationId: getApiV1NotifyUser
      x-api-path-slug: apiv1notifyuserid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Notify
      - Userid
    post:
      summary: Post Notify Userid
      description: Post notify userid.
      operationId: postApiV1NotifyUser
      x-api-path-slug: apiv1notifyuserid-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: notificationIds
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Notify
      - Userid
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