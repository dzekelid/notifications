---
swagger: "2.0"
x-collection-name: AWS Glacier
x-complete: 0
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
    delete:
      summary: Delete  Vault  Notifications
      description: "DescriptionThis operation deletes the notification configuration
        set for a vault \n\t\t\tSet Vault Notification Configuration (PUT\n\t\tnotification-configuration).
        The operation is\n\t\t\teventually consistent&#8212;that is, it might take
        some time for Amazon Glacier to\n\t\t\tcompletely disable the notifications,
        and you might still receive some notifications for\n\t\t\ta short time after
        you send the delete request. RequestsTo delete a vault's notification configuration,
        send a DELETE request to the\n\t\t\tvault's notification-configuration subresource."
      operationId: "Delete Vault Notifications (DELETE\n\t\tnotification-configuration)"
      x-api-path-slug: accountidvaultsvaultnamenotificationconfiguration-delete
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
        200:
          description: OK
      tags:
      - Vault Notifications
    get:
      summary: Get  Vault  Notifications
      description: "DescriptionThis operation retrieves the notification-configuration
        subresource set on the\n\t\t\tvault (see Set Vault Notification Configuration
        (PUT\n\t\tnotification-configuration). If notification configuration for a\n\t\t\tvault
        is not set, the operation returns a 404 Not Found error. For more\n\t\t\tinformation
        about vault notifications, see Configuring Vault Notifications in Amazon Glacier.
        RequestsTo retrieve the notification configuration information, send a GET
        request to\n\t\t\tthe URI of a vault's notification-configuration subresource."
      operationId: "Get Vault Notifications (GET\n\t\tnotification-configuration)"
      x-api-path-slug: accountidvaultsvaultnamenotificationconfiguration-get
      parameters:
      - in: query
        name: Events
        description: A list of one or more events for which Amazon Glacier will send
          a notification to thespecified Amazon SNS topic
        type: string
      - in: query
        name: SNSTopic
        description: The Amazon Simple Notification Service (Amazon SNS) topic Amazon
          Resource Name (ARN)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Vault Notifications
    put:
      summary: Set  Vault  Notification  Configuration
      description: "DescriptionRetrieving an archive and a vault inventory are asynchronous
        operations in Amazon Glacier for which\n\t\t\tyou must first initiate a job
        and wait for the job to complete before you can download\n\t\t\tthe job output.
        Most Amazon Glacier jobs take about four hours to complete. You can configure
        a\n\t\t\tvault to post a message to an Amazon Simple Notification Service
        (Amazon SNS) topic when these jobs complete. You can\n\t\t\tuse this operation
        to set notification configuration on the vault. For more information,\n\t\t\tsee
        Configuring Vault Notifications in Amazon Glacier.\n\t\t\t\n\t\tTo configure
        vault notifications, send a PUT request to the\n\t\t\t\tnotification-configuration
        subresource of the vault. A notification\n\t\t\tconfiguration is specific
        to a vault; therefore, it is also referred to as a vault\n\t\t\tsubresource.
        The request should include a JSON document that provides an Amazon Simple
        Notification Service (Amazon SNS) topic and the events for which you want
        Amazon Glacier to\n\t\t\tsend notifications to the topic.You can configure
        a vault to publish a notification for the following vault events:\n\t\t\tArchiveRetrievalCompleted&#8212;
        This event\n\t\t\t\t\t\toccurs when a job that was initiated for an archive
        retrieval is completed\n\t\t\t\t\t\t\t(Initiate Job (POST jobs)). The status
        of the completed\n\t\t\t\t\t\tjob can be Succeeded or Failed. The notification\n\t\t\t\t\t\tsent
        to the SNS topic is the same output as returned from Describe Job (GET JobID).InventoryRetrievalCompleted&#8212;
        This event\n\t\t\t\t\t\toccurs when a job that was initiated for an inventory
        retrieval is completed\n\t\t\t\t\t\t\t(Initiate Job (POST jobs)). The status
        of the completed\n\t\t\t\t\t\tjob can be Succeeded or Failed. The notification\n\t\t\t\t\t\tsent
        to the SNS topic is the same output as returned from Describe Job (GET JobID).\n\t\tAmazon
        SNS topics must grant permission to the vault to be allowed to publish notifications\n\t\t\tto
        the topic.RequestsTo set notification configuration on your vault, send a
        PUT request to the URI of the\n\t\t\tvault's notification-configuration subresource.
        You specify the\n\t\t\tconfiguration in the request body. The configuration
        includes the Amazon SNS topic name\n\t\t\tand an array of events that trigger
        notification to each topic."
      operationId: "Set Vault Notification Configuration (PUT\n\t\tnotification-configuration)"
      x-api-path-slug: accountidvaultsvaultnamenotificationconfiguration-put
      parameters:
      - in: query
        name: Events
        description: An array of one or more events for which you want Amazon Glacier
          to sendnotification
        type: string
      - in: query
        name: SNSTopic
        description: The Amazon SNS topic ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Vault Notifications
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