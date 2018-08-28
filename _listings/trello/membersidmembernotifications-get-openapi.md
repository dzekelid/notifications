---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Get Members Notifications
  description: Get members notifications.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /members/{idMember}/notifications:
    get:
      summary: Get Members Notifications
      description: Get members notifications.
      operationId: getMembersNotificationsByIdMember
      x-api-path-slug: membersidmembernotifications-get
      parameters:
      - in: query
        name: before
        description: An id, or null
      - in: query
        name: display
        description: true or false
      - in: query
        name: entities
        description: true or false
      - in: query
        name: fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator,
          type or unread'
      - in: query
        name: filter
        description: 'all or a comma-separated list of: addAdminToBoard, addAdminToOrganization,
          addedAttachmentToCard, addedMemberToCard, addedToBoard, addedToCard, addedToOrganization,
          cardDueSoon, changeCard, closeBoard, commentCard, createdCard, declinedInvitationToBoard,
          declinedInvitationToOrganization, invitedToBoard, invitedToOrganization,
          makeAdminOfBoard, makeAdminOfOrganization, memberJoinedTrello, mentionedOnCard,
          removedFromBoard, removedFromCard, removedFromOrganization, removedMemberFromCard,
          unconfirmedInvitedToBoard, unconfirmedInvitedToOrganization or updateCheckItemStateOnCard'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 1 to 1000
      - in: query
        name: memberCreator
        description: true or false
      - in: query
        name: memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: page
        description: a number from 0 to 100
      - in: query
        name: read_filter
        description: 'One of: all, read or unread'
      - in: query
        name: since
        description: An id, or null
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
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