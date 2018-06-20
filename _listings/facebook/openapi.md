---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  description: connect-to-the-social-network-with-the-graph-api-
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
---