---
swagger: "2.0"
info:
  title: Meetup Read Notifications
  description: Marks groups of [notifications](/meetup_api/docs/notifications/) as
    read.
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
  /notifications/read:
    post:
      summary: Read Notifications
      description: Marks groups of [notifications](/meetup_api/docs/notifications/)
        as read
      operationId: notifications
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
      - events
      - notifications
definitions: []
x-collection-name: Meetup
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