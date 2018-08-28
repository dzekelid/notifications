swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 1
info:
  title: AWS Simple Email Service API
  version: 1.0.0
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