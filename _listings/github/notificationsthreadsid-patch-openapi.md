---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Patch Notifications Threads
  description: Mark a thread as read
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
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
      summary: Get Notifications
      description: |-
        List your notifications.
        List all notifications for the current user, grouped by repository.
      operationId: list-your-notificationslist-all-notifications-for-the-current-user-grouped-by-repository
      x-api-path-slug: notifications-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: query
        name: all
        description: True to show notifications marked as read
      - in: query
        name: participating
        description: True to show only notifications in which the user is directly
          participatingor mentioned
      - in: query
        name: since
        description: 'The time should be passed in as UTC in the ISO 8601 format:
          YYYY-MM-DDTHH:MM:SSZ'
      responses:
        200:
          description: OK
      tags:
      - Notifications
    put:
      summary: Put Notifications
      description: |-
        Mark as read.
        Marking a notification as "read" removes it from the default view on GitHub.com.
      operationId: mark-as-readmarking-a-notification-as-read-removes-it-from-the-default-view-on-githubcom
      x-api-path-slug: notifications-put
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /notifications/threads/{id}:
    get:
      summary: Get Notifications Threads
      description: View a single thread.
      operationId: view-a-single-thread
      x-api-path-slug: notificationsthreadsid-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
        description: Id of thread
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Threads
    patch:
      summary: Patch Notifications Threads
      description: Mark a thread as read
      operationId: mark-a-thread-as-read
      x-api-path-slug: notificationsthreadsid-patch
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
        description: Id of thread
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Threads
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