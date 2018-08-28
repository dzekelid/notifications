swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
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