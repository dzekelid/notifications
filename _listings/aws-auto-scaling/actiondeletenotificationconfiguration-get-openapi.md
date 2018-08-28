---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 0
info:
  title: AWS Auto Scaling API Delete Notification Configuration
  version: 1.0.0
  description: Deletes the specified notification.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteNotificationConfiguration:
    get:
      summary: Delete Notification Configuration
      description: Deletes the specified notification.
      operationId: deleteNotificationConfiguration
      x-api-path-slug: actiondeletenotificationconfiguration-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: TopicARN
        description: The Amazon Resource Name (ARN) of the Amazon Simple Notification
          Service (SNS) topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /?Action=DescribeNotificationConfigurations:
    get:
      summary: Describe Notification Configurations
      description: Describes the notification actions associated with the specified
        Auto Scaling group.
      operationId: describeNotificationConfigurations
      x-api-path-slug: actiondescribenotificationconfigurations-get
      parameters:
      - in: query
        name: AutoScalingGroupNames.member.N
        description: The name of the group
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /?Action=PutNotificationConfiguration:
    get:
      summary: Put Notification Configuration
      description: Configures an Auto Scaling group to send notifications when specified
        events take place.
      operationId: putNotificationConfiguration
      x-api-path-slug: actionputnotificationconfiguration-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: NotificationTypes.member.N
        description: The type of event that will cause the notification to be sent
        type: string
      - in: query
        name: TopicARN
        description: The Amazon Resource Name (ARN) of the Amazon Simple Notification
          Service (SNS) topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /?Action=DescribeAutoScalingNotificationTypes:
    get:
      summary: Describe Auto Scaling Notification Types
      description: Describes the notification types that are supported by Auto Scaling.
      operationId: describeAutoScalingNotificationTypes
      x-api-path-slug: actiondescribeautoscalingnotificationtypes-get
      parameters:
      - in: query
        name: AutoScalingNotificationTypes.member.N
        description: The notification types
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Notifications
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