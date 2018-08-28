---
swagger: "2.0"
x-collection-name: Boxcar
x-complete: 0
info:
  title: Box Car Subscribe to Provider
  description: This sends the user with the matching e-mail address a push notification
    which requests that they add your service. This will ease integration with your
    website, as you will have already registered them on your system and can identify
    whom they are based on their Boxcar e-mail address. Please note, this API call
    is an exception and will return an HTTP status code of 404 if we are unable to
    find the registered user by e-mail in our system. If the email address is not
    found in our system, we'll send an email to it letting the user know where they
    can download Boxcar. If the user has already added your service, we'll return
    an HTTP status code of 401.
  version: 1.0.0
host: boxcar.io
basePath: /devices/providers/%7Bprovider_key%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /notifications/subscribe:
    post:
      summary: Subscribe to Provider
      description: This sends the user with the matching e-mail address a push notification
        which requests that they add your service. This will ease integration with
        your website, as you will have already registered them on your system and
        can identify whom they are based on their Boxcar e-mail address. Please note,
        this API call is an exception and will return an HTTP status code of 404 if
        we are unable to find the registered user by e-mail in our system. If the
        email address is not found in our system, we'll send an email to it letting
        the user know where they can download Boxcar. If the user has already added
        your service, we'll return an HTTP status code of 401.
      operationId: Create_subscribeToProvider_
      x-api-path-slug: notificationssubscribe-post
      parameters:
      - in: query
        name: email
        description: The users e-mail address
      - in: query
        name: provider_key
        description: The API key
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Subscriptions
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