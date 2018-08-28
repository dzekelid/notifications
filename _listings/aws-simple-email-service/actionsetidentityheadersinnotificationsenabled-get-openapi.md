---
swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 0
info:
  title: AWS Simple Email Service API Set Identity Headers In Notifications Enabled
  version: 1.0.0
  description: "Given an identity (an email address or a domain), sets whether Amazon
    SES includes \n            the original email headers in the Amazon Simple Notification
    Service (Amazon SNS) notifications \n            of a specified type."
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SetIdentityHeadersInNotificationsEnabled:
    get:
      summary: Set Identity Headers In Notifications Enabled
      description: "Given an identity (an email address or a domain), sets whether
        Amazon SES includes \n            the original email headers in the Amazon
        Simple Notification Service (Amazon SNS) notifications \n            of a
        specified type."
      operationId: setIdentityHeadersInNotificationsEnabled
      x-api-path-slug: actionsetidentityheadersinnotificationsenabled-get
      parameters:
      - in: query
        name: Enabled
        description: Sets whether Amazon SES includes the original email headers in
          Amazon SNS notifications             of the specified notification type
        type: string
      - in: query
        name: Identity
        description: The identity for which to enable or disable headers in notifications
        type: string
      - in: query
        name: NotificationType
        description: The notification type for which to enable or disable headers
          in notifications
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
  /?Action=GetIdentityNotificationAttributes:
    get:
      summary: Get Identity Notification Attributes
      description: Given a list of verified identities (email addresses and/or domains),
        returns a structure describing identity notification attributes.
      operationId: getIdentityNotificationAttributes
      x-api-path-slug: actiongetidentitynotificationattributes-get
      parameters:
      - in: query
        name: Identities.member.N
        description: A list of one or more identities
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
  /?Action=SetIdentityNotificationTopic:
    get:
      summary: Set Identity Notification Topic
      description: |-
        Given an identity (an email address or a domain), sets the Amazon Simple Notification Service (Amazon SNS) topic to which Amazon SES will publish
                bounce, complaint, and/or delivery notifications for emails sent with that identity as the Source.
      operationId: setIdentityNotificationTopic
      x-api-path-slug: actionsetidentitynotificationtopic-get
      parameters:
      - in: query
        name: Identity
        description: The identity for which the Amazon SNS topic will be set
        type: string
      - in: query
        name: NotificationType
        description: The type of notifications that will be published to the specified
          Amazon SNS topic
        type: string
      - in: query
        name: SnsTopic
        description: The Amazon Resource Name (ARN) of the Amazon SNS topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
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