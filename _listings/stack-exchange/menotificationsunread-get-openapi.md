---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange My Notiications Unread
  description: "Returns a user's unread notifications, given an access_token.\n \nThis
    method requires an access_token, with a scope containing \"read_inbox\".\n \nThis
    method returns a list of notifications."
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/notifications:
    get:
      summary: My Notiications
      description: "Returns a user's notifications, given an access_token.\n \nThis
        method requires an access_token, with a scope containing \"read_inbox\".\n
        \nThis method returns a list of notifications."
      operationId: returns-a-users-notifications-given-an-access-token-this-method-requires-an-access-token-with-a-scop
      x-api-path-slug: menotifications-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /me/notifications/unread:
    get:
      summary: My Notiications Unread
      description: "Returns a user's unread notifications, given an access_token.\n
        \nThis method requires an access_token, with a scope containing \"read_inbox\".\n
        \nThis method returns a list of notifications."
      operationId: returns-a-users-unread-notifications-given-an-access-token-this-method-requires-an-access-token-with
      x-api-path-slug: menotificationsunread-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Notifications
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