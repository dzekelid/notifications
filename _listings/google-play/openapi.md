swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /enterprises/acknowledgeNotificationSet:
    post:
      summary: Create Acknowledges Notification Set
      description: Acknowledges notifications that were received from Enterprises.PullNotificationSet
        to prevent subsequent calls from returning the same notifications.
      operationId: androidenterprise.enterprises.acknowledgeNotificationSet
      x-api-path-slug: enterprisesacknowledgenotificationset-post
      parameters:
      - in: query
        name: notificationSetId
        description: The notification set ID as returned by Enterprises
      responses:
        200:
          description: OK
      tags:
      - Notification
  /enterprises/pullNotificationSet:
    post:
      summary: Get Notification Set
      description: |-
        Pulls and returns a notification set for the enterprises associated with the service account authenticated for the request. The notification set may be empty if no notification are pending.
        A notification set returned needs to be acknowledged within 20 seconds by calling Enterprises.AcknowledgeNotificationSet, unless the notification set is empty.
        Notifications that are not acknowledged within the 20 seconds will eventually be included again in the response to another PullNotificationSet request, and those that are never acknowledged will ultimately be deleted according to the Google Cloud Platform Pub/Sub system policy.
        Multiple requests might be performed concurrently to retrieve notifications, in which case the pending notifications (if any) will be split among each caller, if any are pending.
        If no notifications are present, an empty notification list is returned. Subsequent requests may return more notifications once they become available.
      operationId: androidenterprise.enterprises.pullNotificationSet
      x-api-path-slug: enterprisespullnotificationset-post
      parameters:
      - in: query
        name: requestMode
        description: The request mode for pulling notifications
      responses:
        200:
          description: OK
      tags:
      - Notification