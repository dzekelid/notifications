swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/groups/{id}/notification_settings:
    get:
      summary: Get Groups Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: getV3GroupsIdNotificationSettings
      x-api-path-slug: v3groupsidnotification-settings-get
      parameters:
      - in: path
        name: id
        description: The group ID or project ID or project NAMESPACE/PROJECT_NAME
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Notification
      - Settings
    put:
      summary: Put Groups Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: putV3GroupsIdNotificationSettings
      x-api-path-slug: v3groupsidnotification-settings-put
      parameters:
      - in: formData
        name: close_issue
        description: Enable/disable this notification
      - in: formData
        name: close_merge_request
        description: Enable/disable this notification
      - in: formData
        name: failed_pipeline
        description: Enable/disable this notification
      - in: path
        name: id
        description: The group ID or project ID or project NAMESPACE/PROJECT_NAME
      - in: formData
        name: level
        description: The group notification level
      - in: formData
        name: merge_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_issue
        description: Enable/disable this notification
      - in: formData
        name: new_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_note
        description: Enable/disable this notification
      - in: formData
        name: reassign_issue
        description: Enable/disable this notification
      - in: formData
        name: reassign_merge_request
        description: Enable/disable this notification
      - in: formData
        name: reopen_issue
        description: Enable/disable this notification
      - in: formData
        name: reopen_merge_request
        description: Enable/disable this notification
      - in: formData
        name: success_pipeline
        description: Enable/disable this notification
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Notification
      - Settings
  /v3/projects/{id}/notification_settings:
    get:
      summary: Get Projects Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: getV3ProjectsIdNotificationSettings
      x-api-path-slug: v3projectsidnotification-settings-get
      parameters:
      - in: path
        name: id
        description: The group ID or project ID or project NAMESPACE/PROJECT_NAME
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Notification
      - Settings
    put:
      summary: Put Projects Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: putV3ProjectsIdNotificationSettings
      x-api-path-slug: v3projectsidnotification-settings-put
      parameters:
      - in: formData
        name: close_issue
        description: Enable/disable this notification
      - in: formData
        name: close_merge_request
        description: Enable/disable this notification
      - in: formData
        name: failed_pipeline
        description: Enable/disable this notification
      - in: path
        name: id
        description: The group ID or project ID or project NAMESPACE/PROJECT_NAME
      - in: formData
        name: level
        description: The project notification level
      - in: formData
        name: merge_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_issue
        description: Enable/disable this notification
      - in: formData
        name: new_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_note
        description: Enable/disable this notification
      - in: formData
        name: reassign_issue
        description: Enable/disable this notification
      - in: formData
        name: reassign_merge_request
        description: Enable/disable this notification
      - in: formData
        name: reopen_issue
        description: Enable/disable this notification
      - in: formData
        name: reopen_merge_request
        description: Enable/disable this notification
      - in: formData
        name: success_pipeline
        description: Enable/disable this notification
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Notification
      - Settings
  /v3/notification_settings:
    get:
      summary: Get Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: getV3NotificationSettings
      x-api-path-slug: v3notification-settings-get
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Settings
    put:
      summary: Put Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: putV3NotificationSettings
      x-api-path-slug: v3notification-settings-put
      parameters:
      - in: formData
        name: close_issue
        description: Enable/disable this notification
      - in: formData
        name: close_merge_request
        description: Enable/disable this notification
      - in: formData
        name: failed_pipeline
        description: Enable/disable this notification
      - in: formData
        name: level
        description: The global notification level
      - in: formData
        name: merge_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_issue
        description: Enable/disable this notification
      - in: formData
        name: new_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_note
        description: Enable/disable this notification
      - in: formData
        name: notification_email
        description: The email address to send notifications
      - in: formData
        name: reassign_issue
        description: Enable/disable this notification
      - in: formData
        name: reassign_merge_request
        description: Enable/disable this notification
      - in: formData
        name: reopen_issue
        description: Enable/disable this notification
      - in: formData
        name: reopen_merge_request
        description: Enable/disable this notification
      - in: formData
        name: success_pipeline
        description: Enable/disable this notification
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Settings