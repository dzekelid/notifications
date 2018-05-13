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
- name: Amazon Glacier API Delete  Vault  Notifications
  description: "DescriptionThis operation deletes the notification configuration set
    for a vault \n\t\t\tSet Vault Notification Configuration (PUT\n\t\tnotification-configuration).
    The operation is\n\t\t\teventually consistent&#8212;that is, it might take some
    time for Amazon Glacier to\n\t\t\tcompletely disable the notifications, and you
    might still receive some notifications for\n\t\t\ta short time after you send
    the delete request. RequestsTo delete a vault's notification configuration, send
    a DELETE request to the\n\t\t\tvault's notification-configuration subresource."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: http:://{host}//
  tags: Notifications
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/aws-glacier/accountid-vaults-vaultname-notification-configuration-delete.md
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