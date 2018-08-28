---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Get Notifications Notification Board
  description: Get notifications notification board.
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
  /members/{idMember}/notifications/{filter}:
    get:
      summary: Get Members Notifications Filter
      description: Get members notifications filter.
      operationId: getMembersNotificationsByIdMemberByFilter
      x-api-path-slug: membersidmembernotificationsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Notifications
      - Filter
  /notifications/all/read:
    post:
      summary: Post Notifications All Read
      description: Post notifications all read.
      operationId: addNotificationsAllRead
      x-api-path-slug: notificationsallread-post
      parameters:
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - ""
      - Read
  /notifications/{idNotification}:
    get:
      summary: Get Notifications Notification
      description: Get notifications notification.
      operationId: getNotificationsByIdNotification
      x-api-path-slug: notificationsidnotification-get
      parameters:
      - in: query
        name: board
        description: true or false
      - in: query
        name: board_fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: card
        description: true or false
      - in: query
        name: card_fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
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
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: list
        description: true or false
      - in: query
        name: member
        description: true or false
      - in: query
        name: memberCreator
        description: true or false
      - in: query
        name: memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: organization
        description: true or false
      - in: query
        name: organization_fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
    put:
      summary: Put Notifications Notification
      description: Put notifications notification.
      operationId: updateNotificationsByIdNotification
      x-api-path-slug: notificationsidnotification-put
      parameters:
      - in: body
        name: body
        description: Attributes of Notifications to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
  /notifications/{idNotification}/board:
    get:
      summary: Get Notifications Notification Board
      description: Get notifications notification board.
      operationId: getNotificationsBoardByIdNotification
      x-api-path-slug: notificationsidnotificationboard-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Board
  /notifications/{idNotification}/board/{field}:
    get:
      summary: Get Notifications Notification Board Field
      description: Get notifications notification board field.
      operationId: getNotificationsBoardByIdNotificationByField
      x-api-path-slug: notificationsidnotificationboardfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Board
      - Field
  /notifications/{idNotification}/card:
    get:
      summary: Get Notifications Notification Card
      description: Get notifications notification card.
      operationId: getNotificationsCardByIdNotification
      x-api-path-slug: notificationsidnotificationcard-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Card
  /notifications/{idNotification}/card/{field}:
    get:
      summary: Get Notifications Notification Card Field
      description: Get notifications notification card field.
      operationId: getNotificationsCardByIdNotificationByField
      x-api-path-slug: notificationsidnotificationcardfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Card
      - Field
  /notifications/{idNotification}/display:
    get:
      summary: Get Notifications Notification Display
      description: Get notifications notification display.
      operationId: getNotificationsDisplayByIdNotification
      x-api-path-slug: notificationsidnotificationdisplay-get
      parameters:
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Display
  /notifications/{idNotification}/entities:
    get:
      summary: Get Notifications Notification Entities
      description: Get notifications notification entities.
      operationId: getNotificationsEntitiesByIdNotification
      x-api-path-slug: notificationsidnotificationentities-get
      parameters:
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Entities
  /notifications/{idNotification}/list:
    get:
      summary: Get Notifications Notification List
      description: Get notifications notification list.
      operationId: getNotificationsListByIdNotification
      x-api-path-slug: notificationsidnotificationlist-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - List
  /notifications/{idNotification}/list/{field}:
    get:
      summary: Get Notifications Notification List Field
      description: Get notifications notification list field.
      operationId: getNotificationsListByIdNotificationByField
      x-api-path-slug: notificationsidnotificationlistfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - List
      - Field
  /notifications/{idNotification}/member:
    get:
      summary: Get Notifications Notification Member
      description: Get notifications notification member.
      operationId: getNotificationsMemberByIdNotification
      x-api-path-slug: notificationsidnotificationmember-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, avatarSource,
          bio, bioData, confirmed, email, fullName, gravatarHash, idBoards, idBoardsPinned,
          idOrganizations, idPremOrgsAdmin, initials, loginTypes, memberType, oneTimeMessagesDismissed,
          prefs, premiumFeatures, products, status, status, trophies, uploadedAvatarHash,
          url or username'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Member
  /notifications/{idNotification}/member/{field}:
    get:
      summary: Get Notifications Notification Member Field
      description: Get notifications notification member field.
      operationId: getNotificationsMemberByIdNotificationByField
      x-api-path-slug: notificationsidnotificationmemberfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Member
      - Field
  /notifications/{idNotification}/memberCreator:
    get:
      summary: Get Notifications Notification Member Creator
      description: Get notifications notification member creator.
      operationId: getNotificationsMemberCreatorByIdNotification
      x-api-path-slug: notificationsidnotificationmembercreator-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, avatarSource,
          bio, bioData, confirmed, email, fullName, gravatarHash, idBoards, idBoardsPinned,
          idOrganizations, idPremOrgsAdmin, initials, loginTypes, memberType, oneTimeMessagesDismissed,
          prefs, premiumFeatures, products, status, status, trophies, uploadedAvatarHash,
          url or username'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Member
      - Creator
  /notifications/{idNotification}/memberCreator/{field}:
    get:
      summary: Get Notifications Notification Member Creator Field
      description: Get notifications notification member creator field.
      operationId: getNotificationsMemberCreatorByIdNotificationByField
      x-api-path-slug: notificationsidnotificationmembercreatorfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Member
      - Creator
      - Field
  /notifications/{idNotification}/organization:
    get:
      summary: Get Notifications Notification Organization
      description: Get notifications notification organization.
      operationId: getNotificationsOrganizationByIdNotification
      x-api-path-slug: notificationsidnotificationorganization-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Organization
  /notifications/{idNotification}/organization/{field}:
    get:
      summary: Get Notifications Notification Organization Field
      description: Get notifications notification organization field.
      operationId: getNotificationsOrganizationByIdNotificationByField
      x-api-path-slug: notificationsidnotificationorganizationfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Organization
      - Field
  /notifications/{idNotification}/unread:
    put:
      summary: Put Notifications Notification Unread
      description: Put notifications notification unread.
      operationId: updateNotificationsUnreadByIdNotification
      x-api-path-slug: notificationsidnotificationunread-put
      parameters:
      - in: body
        name: body
        description: Attributes of Notifications Unread to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Unread
  /notifications/{idNotification}/{field}:
    get:
      summary: Get Notifications Notification Field
      description: Get notifications notification field.
      operationId: getNotificationsByIdNotificationByField
      x-api-path-slug: notificationsidnotificationfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Field
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