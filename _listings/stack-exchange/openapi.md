swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 1
info:
  title: Stack Exchange
  description: stack-exchange-is-a-network-of-130-qa-communities-including-stack-overflow-
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
  /notifications:
    get:
      summary: Get Notifications
      description: "Returns a user's notifications.\n \nThis method requires an access_token,
        with a scope containing \"read_inbox\".\n \nThis method returns a list of
        notifications."
      operationId: returns-a-users-notifications-this-method-requires-an-access-token-with-a-scope-containing-read-inbo
      x-api-path-slug: notifications-get
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
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /notifications/unread:
    get:
      summary: Get Notifications Unread
      description: "Returns a user's unread notifications.\n \nThis method requires
        an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
        a list of notifications."
      operationId: returns-a-users-unread-notifications-this-method-requires-an-access-token-with-a-scope-containing-re
      x-api-path-slug: notificationsunread-get
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
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /users/{id}/notifications:
    get:
      summary: Get User Notifications
      description: "Returns a user's notifications.\n \nThis method requires an access_token,
        with a scope containing \"read_inbox\".\n \nThis method returns a list of
        notifications."
      operationId: returns-a-users-notifications-this-method-requires-an-access-token-with-a-scope-containing-read-inbo
      x-api-path-slug: usersidnotifications-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
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
      - Users
      - Notifications
  /users/{id}/notifications/unread:
    get:
      summary: Get User Notifications Unread
      description: "Returns a user's unread notifications.\n \nThis method requires
        an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
        a list of notifications."
      operationId: returns-a-users-unread-notifications-this-method-requires-an-access-token-with-a-scope-containing-re
      x-api-path-slug: usersidnotificationsunread-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
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
      - Users
      - Notifications