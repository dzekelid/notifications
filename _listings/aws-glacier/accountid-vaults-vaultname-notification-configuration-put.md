---
swagger: "2.0"
info:
  title: Amazon Glacier API Set  Vault  Notification  Configuration
  version: 1.0.0
  description: "DescriptionRetrieving an archive and a vault inventory are asynchronous
    operations in Amazon Glacier for which\n\t\t\tyou must first initiate a job and
    wait for the job to complete before you can download\n\t\t\tthe job output. Most
    Amazon Glacier jobs take about four hours to complete. You can configure a\n\t\t\tvault
    to post a message to an Amazon Simple Notification Service (Amazon SNS) topic
    when these jobs complete. You can\n\t\t\tuse this operation to set notification
    configuration on the vault. For more information,\n\t\t\tsee Configuring Vault
    Notifications in Amazon Glacier.\n\t\t\t\n\t\tTo configure vault notifications,
    send a PUT request to the\n\t\t\t\tnotification-configuration subresource of the
    vault. A notification\n\t\t\tconfiguration is specific to a vault; therefore,
    it is also referred to as a vault\n\t\t\tsubresource. The request should include
    a JSON document that provides an Amazon Simple Notification Service (Amazon SNS)
    topic and the events for which you want Amazon Glacier to\n\t\t\tsend notifications
    to the topic.You can configure a vault to publish a notification for the following
    vault events:\n\t\t\tArchiveRetrievalCompleted&#8212; This event\n\t\t\t\t\t\toccurs
    when a job that was initiated for an archive retrieval is completed\n\t\t\t\t\t\t\t(Initiate
    Job (POST jobs)). The status of the completed\n\t\t\t\t\t\tjob can be Succeeded
    or Failed. The notification\n\t\t\t\t\t\tsent to the SNS topic is the same output
    as returned from Describe Job (GET JobID).InventoryRetrievalCompleted&#8212; This
    event\n\t\t\t\t\t\toccurs when a job that was initiated for an inventory retrieval
    is completed\n\t\t\t\t\t\t\t(Initiate Job (POST jobs)). The status of the completed\n\t\t\t\t\t\tjob
    can be Succeeded or Failed. The notification\n\t\t\t\t\t\tsent to the SNS topic
    is the same output as returned from Describe Job (GET JobID).\n\t\tAmazon SNS
    topics must grant permission to the vault to be allowed to publish notifications\n\t\t\tto
    the topic.RequestsTo set notification configuration on your vault, send a PUT
    request to the URI of the\n\t\t\tvault's notification-configuration subresource.
    You specify the\n\t\t\tconfiguration in the request body. The configuration includes
    the Amazon SNS topic name\n\t\t\tand an array of events that trigger notification
    to each topic."
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{AccountId}/vaults/{VaultName}/notification-configuration:
    put:
      summary: Set  Vault  Notification  Configuration
      description: "DescriptionRetrieving an archive and a vault inventory are asynchronous
        operations in Amazon Glacier for which\n\t\t\tyou must first initiate a job
        and wait for the job to complete before you can download\n\t\t\tthe job output"
      operationId: "Set Vault Notification Configuration (PUT\n\t\tnotification-configuration)"
      parameters:
      - in: query
        name: Events
        description: "An array of one or more events for which you want Amazon Glacier
          to send\t\t\t\t\t\t\tnotification"
        type: string
      - in: query
        name: SNSTopic
        description: The Amazon SNS topic ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - vault notifications
definitions: []
x-collection-name: AWS Glacier
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