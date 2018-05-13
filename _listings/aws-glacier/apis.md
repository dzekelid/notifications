---
name: AWS Glacier
description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
  service for data archiving and long-term backup. Customers can reliably store large
  or small amounts of data for as little as $0.004 per gigabyte per month, a significant
  savings compared to on-premises solutions. To keep costs low yet suitable for varying
  retrieval needs, Amazon Glacier provides three options for access to archives, from
  a few minutes to several hours.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Storage
- Stack Network
- Amazon Web Services
created: "2018-03-23"
modified: "2018-03-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/aws-glacier/apis.yaml
specificationVersion: "0.14"
apis:
- name: Amazon Glacier API
  description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
    service for data archiving and long-term backup
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: ""
  baseURL: :///
  tags: Notifications
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/aws-glacier/accountid-vaults-vaultname-notification-configuration-put.md
- name: Amazon Glacier API Set  Vault  Notification  Configuration
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
  baseURL: http:://{host}//
  tags: Notifications
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/aws-glacier/accountid-vaults-vaultname-notification-configuration-put.md
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