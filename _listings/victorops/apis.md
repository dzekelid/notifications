---
name: VictorOps
x-slug: victorops
description: VictorOps incident managament software gives DevOps observability, collaboration,
  & real-time alerting, to build, deploy, & operate software. Learn more.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
x-kinRank: "8"
x-alexaRank: "196587"
tags: Notifications
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/victorops/apis.md
specificationVersion: "0.14"
apis:
- name: Victor Ops - Get the available notification types
  x-api-slug: apipublicv1policiestypesnotifications-get
  description: |-
    Get the available notification types

    description: "Send a push notification to all my devices", type: "push"
    description: "Send an email to an email address", type: "email"
    description: "Send an SMS to a phone number", type: "sms"
    description: "Make a phone call to a phone number", type: "phone"

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com//
  tags: Orchestration, Stack Network, Technology, SaaS, Enterprise, internet, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/victorops/apipublicv1policiestypesnotifications-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/victorops/apipublicv1policiestypesnotifications-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://vestorly.api.gallery.streamdata.io
- type: x-api-stack
  url: http://victorops.stack.network
- type: x-blog
  url: https://victorops.com/blog/
- type: x-blog-rss
  url: https://victorops.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/victorops
- type: x-email
  url: support@victorops.com
- type: x-email
  url: info@victorops.com
- type: x-email
  url: press@victorops.com
- type: x-email
  url: sales@victorops.com
- type: x-github
  url: https://github.com/victorops
- type: x-openapi
  url: https://portal.victorops.com/api-docs/victorops-api-v1.yaml
- type: x-pricing
  url: https://victorops.com/pricing/
- type: x-twitter
  url: https://twitter.com/VictorOps
- type: x-website
  url: http://victorops.com
- type: x-website
  url: https://victorops.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---