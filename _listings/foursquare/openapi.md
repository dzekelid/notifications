---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
  description: checkin-explore-your-city-and-connect-people-and-places-bapi-v2-b
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /updates/marknotificationsread:
    post:
      summary: Post Updates Marknotificationsread
      description: /updates/notifications
      operationId: updatesnotifications
      x-api-path-slug: updatesmarknotificationsread-post
      parameters:
      - in: query
        name: highWatermark
        description: The timestamp of the most recent notification that the user viewed
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - S
      - Marknotificationsread
  /updates/notifications:
    get:
      summary: Get Updates Notifications
      description: /updates/{UPDATE_ID}
      operationId: updatesupdate-id
      x-api-path-slug: updatesnotifications-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of results to return, up to 99
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - S
      - Notifications
---