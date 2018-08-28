---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Record that the feedback for a Valuation was notified to the vendor.
  version: 1.0.0
  description: Record that the feedback for a valuation was notified to the vendor..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/people/sendnotification:
    post:
      summary: Sends a user notification to the specified user
      description: Sends a user notification to the specified user.
      operationId: People_SendNotificationBysendNotificationToPerson
      x-api-path-slug: apipeoplesendnotification-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: sendNotificationToPerson
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sends
      - User
      - Notification
      - To
      - Specified
      - User
  /api/admin/system/sendNotificationToAllUsersInAgency:
    post:
      summary: Send a live notification to all active users in an agency
      description: Send a live notification to all active users in an agency.
      operationId: System_SendNotificationToAgencyUsersByagencyIdBysendNotification
      x-api-path-slug: apiadminsystemsendnotificationtoallusersinagency-post
      parameters:
      - in: query
        name: agencyId
        description: The agency identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: sendNotification
        description: The send notification
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Send
      - Live
      - Notification
      - To
      - ""
      - Active
      - Users
      - In
      - Agency
  /api/valuation/{valuationId}/feedbacknotified:
    post:
      summary: Record that the feedback for a Valuation was notified to the vendor.
      description: Record that the feedback for a valuation was notified to the vendor..
      operationId: Valuation_FeedbackNotifiedByvaluationIdBynotifiedDateBynegotiatorIdsByvendorNotified
      x-api-path-slug: apivaluationvaluationidfeedbacknotified-post
      parameters:
      - in: query
        name: negotiatorIds
        description: The negotiator(s) who notified the vendor
      - in: query
        name: notifiedDate
        description: The date the vendor was notified
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: valuationId
        description: valuation id
      - in: query
        name: vendorNotified
        description: Whether or not the vendor has been notified
      responses:
        200:
          description: OK
      tags:
      - Record
      - That
      - Feedbacka
      - Valuation
      - Was
      - Notified
      - To
      - Vendor
  /api/viewing/{viewingFeedbackId}/feedbacknotified:
    post:
      summary: Record that the feedback for a Viewing was notified to the vendor.
      description: Record that the feedback for a viewing was notified to the vendor..
      operationId: Viewing_FeedbackNotifiedByviewingFeedbackIdBytypeBynotifiedDateBynegIds
      x-api-path-slug: apiviewingviewingfeedbackidfeedbacknotified-post
      parameters:
      - in: query
        name: negIds
      - in: query
        name: notifiedDate
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: type
        description: Task type for how vendor was communicated e
      - in: path
        name: viewingFeedbackId
        description: viewing feedback id
      responses:
        200:
          description: OK
      tags:
      - Record
      - That
      - Feedbacka
      - Viewing
      - Was
      - Notified
      - To
      - Vendor
  /api/viewing/{viewingFeedbackId}/editfeedbacknotified:
    put:
      summary: Edit that the feedback for a Viewing was notified to the vendor.
      description: Edit that the feedback for a viewing was notified to the vendor..
      operationId: Viewing_EditFeedbackNotifiedByviewingFeedbackIdByvendorNotifiedIdBytypeBynotifiedDateBynegIds
      x-api-path-slug: apiviewingviewingfeedbackideditfeedbacknotified-put
      parameters:
      - in: query
        name: negIds
      - in: query
        name: notifiedDate
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: type
        description: Task type for how vendor was communicated e
      - in: query
        name: vendorNotifiedId
        description: vendor notified id
      - in: path
        name: viewingFeedbackId
        description: viewing feedback id
      responses:
        200:
          description: OK
      tags:
      - Edit
      - That
      - Feedbacka
      - Viewing
      - Was
      - Notified
      - To
      - Vendor
  /api/documentgeneration/offerwithdrawn:
    post:
      summary: Generates a correspondence to notify any parties of the withdrawl of
        an offer.  Uses default values where possible.
      description: Generates a correspondence to notify any parties of the withdrawl
        of an offer.  uses default values where possible..
      operationId: DocumentGeneration_OfferwithdrawnLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferwithdrawn-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Withdrawl
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/completed:
    post:
      summary: Generates a correspondence to notify any parties of completion.  Uses
        default values where possible.
      description: Generates a correspondence to notify any parties of completion.  uses
        default values where possible..
      operationId: DocumentGeneration_CompletedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcompleted-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Completion
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/exchanged:
    post:
      summary: Generates a correspondence to notify any parties of exchanged.  Uses
        default values where possible.
      description: Generates a correspondence to notify any parties of exchanged.  uses
        default values where possible..
      operationId: DocumentGeneration_ExchangedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationexchanged-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Exchanged
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/confirmationofviewing:
    post:
      summary: Generates a correspondence to notify all parties of a scheduled viewing.  Uses
        default values where possible.
      description: Generates a correspondence to notify all parties of a scheduled
        viewing.  uses default values where possible..
      operationId: DocumentGeneration_ConfirmationOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmationofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - ""
      - Parties
      - Of
      - Scheduled
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/cancellationofviewing:
    post:
      summary: Generates a correspondence to notify parties of a cancellation of a
        viewing.  Uses default values where possible.
      description: Generates a correspondence to notify parties of a cancellation
        of a viewing.  uses default values where possible..
      operationId: DocumentGeneration_CancellationOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancellationofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Parties
      - Of
      - Cancellation
      - Of
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/reschedulingofviewing:
    post:
      summary: Generates a correspondence to notify parties involved of a rescheduling
        of a viewing.  Uses default values where possible.
      description: Generates a correspondence to notify parties involved of a rescheduling
        of a viewing.  uses default values where possible..
      operationId: DocumentGeneration_ReschedulingOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationreschedulingofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Parties
      - Involved
      - Of
      - Rescheduling
      - Of
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offer:
    post:
      summary: Generates a correspondence notifying the vendor of an offer.  Uses
        default values where possible.
      description: Generates a correspondence notifying the vendor of an offer.  uses
        default values where possible..
      operationId: DocumentGeneration_OfferLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationoffer-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Notifying
      - Vendor
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
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