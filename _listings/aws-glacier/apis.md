---
name: AWS Glacier
x-slug: aws-glacier
description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
  service for data archiving and long-term backup. Customers can reliably store large
  or small amounts of data for as little as $0.004 per gigabyte per month, a significant
  savings compared to on-premises solutions. To keep costs low yet suitable for varying
  retrieval needs, Amazon Glacier provides three options for access to archives, from
  a few minutes to several hours.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Notifications
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/aws-glacier/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Glacier API Delete  Vault  Notifications
  x-api-slug: amazon-glacier-api
  description: "DescriptionThis operation deletes the notification configuration set
    for a vault \n\t\t\tSet Vault Notification Configuration (PUT\n\t\tnotification-configuration).
    The operation is\n\t\t\teventually consistent&#8212;that is, it might take some
    time for Amazon Glacier to\n\t\t\tcompletely disable the notifications, and you
    might still receive some notifications for\n\t\t\ta short time after you send
    the delete request. RequestsTo delete a vault's notification configuration, send
    a DELETE request to the\n\t\t\tvault's notification-configuration subresource."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults/{VaultName}/notification-configuration
  tags: Vault Notifications
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/aws-glacier/accountidvaultsvaultnamenotificationconfiguration-delete-openapi.md
- name: Amazon Glacier API Get  Vault  Notifications
  x-api-slug: amazon-glacier-api
  description: "DescriptionThis operation retrieves the notification-configuration
    subresource set on the\n\t\t\tvault (see Set Vault Notification Configuration
    (PUT\n\t\tnotification-configuration). If notification configuration for a\n\t\t\tvault
    is not set, the operation returns a 404 Not Found error. For more\n\t\t\tinformation
    about vault notifications, see Configuring Vault Notifications in Amazon Glacier.
    RequestsTo retrieve the notification configuration information, send a GET request
    to\n\t\t\tthe URI of a vault's notification-configuration subresource."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults/{VaultName}/notification-configuration
  tags: Vault Notifications
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/aws-glacier/accountidvaultsvaultnamenotificationconfiguration-get-openapi.md
- name: Amazon Glacier API Set  Vault  Notification  Configuration
  x-api-slug: amazon-glacier-api
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults/{VaultName}/notification-configuration
  tags: Vault Notifications
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/aws-glacier/accountidvaultsvaultnamenotificationconfiguration-put-openapi.md
- name: Amazon Glacier API
  x-api-slug: amazon-glacier-api
  description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
    service for data archiving and long-term backup. Customers can reliably store
    large or small amounts of data for as little as $0.004 per gigabyte per month,
    a significant savings compared to on-premises solutions. To keep costs low yet
    suitable for varying retrieval needs, Amazon Glacier provides three options for
    access to archives, from a few minutes to several hours.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: :///
  tags: Notifications
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/aws-glacier/openapi.md
x-common:
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/Amazon-Glacier/
- type: x-documentation
  url: http://docs.aws.amazon.com/amazonglacier/latest/dev/amazon-glacier-api.html
- type: x-faq
  url: https://aws.amazon.com/glacier/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=140
- type: x-getting-started
  url: https://aws.amazon.com/glacier/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/glacier/pricing/
- type: x-website
  url: https://aws.amazon.com/glacier/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---