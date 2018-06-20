---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 0
info:
  title: Victor Ops Get the available notification types
  description: |-
    Get the available notification types

    description: "Send a push notification to all my devices", type: "push"
    description: "Send an email to an email address", type: "email"
    description: "Send an SMS to a phone number", type: "sms"
    description: "Make a phone call to a phone number", type: "phone"

    This API may be called a maximum of 15 times per minute.
  version: 0.0.2
host: api.victorops.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-public/v1/policies/types/notifications:
    get:
      summary: Get the available notification types
      description: |-
        Get the available notification types

        description: "Send a push notification to all my devices", type: "push"
        description: "Send an email to an email address", type: "email"
        description: "Send an SMS to a phone number", type: "sms"
        description: "Make a phone call to a phone number", type: "phone"

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.policies.types.notifications.get
      x-api-path-slug: apipublicv1policiestypesnotifications-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Policies
      - Types
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