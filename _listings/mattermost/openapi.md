---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost API Reference
  description: -api-v4-is-stable-with-the-mattermost-server-4-0-release--api-v3-was-deprecated-on-january-16th-2018-and-scheduled-for-removal-in-mattermost-v5-0--details-heretagapiv3deprecation--looking-for-the-api-v3-reference-it-has-moved-herehttpsapi-mattermost-comv3-
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /channels/{channel_id}/members/{user_id}/notify_props:
    put:
      summary: Update channel notifications
      description: |-
        Update a user's notification properties for a channel. Only the provided fields are updated.
        ##### Permissions
        Must be logged in as the user or have `edit_other_users` permission.
      operationId: update-a-users-notification-properties-for-a-channel-only-the-provided-fields-are-updated-permission
      x-api-path-slug: channelschannel-idmembersuser-idnotify-props-put
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: body
        name: notify_props
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
      - Notifications
---