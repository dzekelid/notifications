---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Notification Search
  description: Search this users Notifications
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /notification:
    get:
      summary: Notification Search
      description: Search this users Notifications
      operationId: notificationSearch
      x-api-path-slug: notification-get
      parameters:
      - in: formData
        name: notificationId
        description: Filter by Notification Id
      - in: formData
        name: subject
        description: Filter by Subject
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Search
    post:
      summary: Notification Add
      description: Add a Notification
      operationId: notificationAdd
      x-api-path-slug: notification-post
      parameters:
      - in: formData
        name: body
        description: The Body
      - in: formData
        name: displayGroupIds
        description: The display group ids to assign this notification to
      - in: formData
        name: isEmail
        description: Flag indicating whether this notification should be emailed
      - in: formData
        name: isInterrupt
        description: Flag indication whether this notification should interrupt the
          web portal nativation/login
      - in: formData
        name: releaseDt
        description: ISO date representing the release date for this notification
      - in: formData
        name: subject
        description: The Subject
      - in: formData
        name: userGroupIds
        description: The user group ids to assign to this notification
      responses:
        200:
          description: OK
      tags:
      - Notification
  /notification/{notificationId}:
    put:
      summary: Notification Edit
      description: Edit a Notification
      operationId: notificationEdit
      x-api-path-slug: notificationnotificationid-put
      parameters:
      - in: formData
        name: body
        description: The Body
      - in: formData
        name: displayGroupIds
        description: The display group ids to assign this notification to
      - in: formData
        name: isEmail
        description: Flag indicating whether this notification should be emailed
      - in: formData
        name: isInterrupt
        description: Flag indication whether this notification should interrupt the
          web portal nativation/login
      - in: path
        name: notificationId
        description: The NotificationId
      - in: formData
        name: releaseDt
        description: ISO date representing the release date for this notification
      - in: formData
        name: subject
        description: The Subject
      - in: formData
        name: userGroupIds
        description: The user group ids to assign to this notification
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Edit
    delete:
      summary: Delete Notification
      description: Delete the provided notification
      operationId: notificationDelete
      x-api-path-slug: notificationnotificationid-delete
      parameters:
      - in: path
        name: notificationId
        description: The Notification Id to Delete
      responses:
        200:
          description: OK
      tags:
      - Notification
  /playlist/widget/notificationview/{playlistId}:
    post:
      summary: Add a Notification Widget
      description: Add a new Notification Widget to the specified playlist
      operationId: WidgetNotificationAdd
      x-api-path-slug: playlistwidgetnotificationviewplaylistid-post
      parameters:
      - in: formData
        name: age
        description: The maximum notification age in minutes - 0 for all
      - in: formData
        name: duration
        description: The Widget Duration
      - in: formData
        name: durationIsPerItem
        description: A flag (0, 1), The duration specified is per page/item, otherwise
          the widget duration is divided between the number of pages/items
      - in: formData
        name: effect
        description: 'Effect that will be used to transitions between items, available
          options: fade, fadeout, scrollVert, scollHorz, flipVert, flipHorz, shuffle,
          tileSlide, tileBlind'
      - in: formData
        name: embedStyle
        description: Custom Style Sheets (CSS)
      - in: formData
        name: name
        description: Optional Widget Name
      - in: formData
        name: noDataMessage
        description: Message to show when no notifications are available
      - in: path
        name: playlistId
        description: The playlist ID to add an Notification Widget
      - in: formData
        name: speed
        description: The transition speed of the selected effect in milliseconds (1000
          = normal)
      - in: formData
        name: useDuration
        description: (0, 1) Select 1 only if you will provide duration parameter as
          well
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Widget
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