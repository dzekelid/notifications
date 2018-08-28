swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{user}/notifications:
    get:
      summary: Get User Notifications
      description: The user's notifications
      operationId: getUserNotifications
      x-api-path-slug: usernotifications-get
      parameters:
      - in: query
        name: include_read
        description: Enables you to see notifications that the user has already read
          in addition to the ones which are unread
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Notifications
  /{notification}:
    post:
      summary: Post Notification
      description: Marks the notification as read
      operationId: postNotification
      x-api-path-slug: notification-post
      parameters:
      - in: path
        name: notification
        description: Represents the ID of the notification
      - in: query
        name: unread
        description: Connect to the social network with the Graph API
      responses:
        200:
          description: OK
      tags:
      - Notification