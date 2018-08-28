swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /notifications:
    get:
      summary: Notifications
      description: Returns all recent Meetup notifications for the authorized member.
        To mark notifications read use [/notifications/read](/meetup_api/docs/notifications/read/)
        endpoint. To get the authenticated Member's current unread count, request
        it in an [HTTP header](/meetup_api/docs/#meta-headers).
      operationId: notifications
      x-api-path-slug: notifications-get
      parameters:
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Notifications
  /notifications/read:
    post:
      summary: Read Notifications
      description: Marks groups of [notifications](/meetup_api/docs/notifications/)
        as read.
      operationId: notifications
      x-api-path-slug: notificationsread-post
      parameters:
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: since_id
        description: The id of the newest notification item, typically the first in
          the list returned by the notifications endpoint
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Notifications
  /notifications/clicked:
    post:
      summary: Clicked Notifications
      description: Marks groups of [notifications](/meetup_api/docs/notifications/)
        as clicked.
      operationId: notifications
      x-api-path-slug: notificationsclicked-post
      parameters:
      - in: query
        name: notif_id
        description: The id of the notification to set as clicked
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Notifications