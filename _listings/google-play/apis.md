---
name: Google Play
x-slug: google-play
description: 'The Google Play Developer API allows you to perform a number of publishing
  and app-management tasks. It includes two components: The Subscriptions and In-App
  Purchases API lets you manage in-app purchases and subscriptions. The Publishing
  API lets you upload and publish apps, and perform other publishing-related tasks.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Notifications
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/google-play/apis.md
specificationVersion: "0.14"
apis:
- name: Google Play - Create Acknowledges Notification Set
  x-api-slug: enterprisesacknowledgenotificationset-post
  description: Acknowledges notifications that were received from Enterprises.PullNotificationSet
    to prevent subsequent calls from returning the same notifications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/google-play/enterprisesacknowledgenotificationset-post-openapi.md
- name: Google Play - Get Notification Set
  x-api-slug: enterprisespullnotificationset-post
  description: |-
    Pulls and returns a notification set for the enterprises associated with the service account authenticated for the request. The notification set may be empty if no notification are pending.
    A notification set returned needs to be acknowledged within 20 seconds by calling Enterprises.AcknowledgeNotificationSet, unless the notification set is empty.
    Notifications that are not acknowledged within the 20 seconds will eventually be included again in the response to another PullNotificationSet request, and those that are never acknowledged will ultimately be deleted according to the Google Cloud Platform Pub/Sub system policy.
    Multiple requests might be performed concurrently to retrieve notifications, in which case the pending notifications (if any) will be split among each caller, if any are pending.
    If no notifications are present, an empty notification list is returned. Subsequent requests may return more notifications once they become available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/google-play/enterprisespullnotificationset-post-openapi.md
- name: Google Play - Create Acknowledges Notification Set
  x-api-slug: enterprisesacknowledgenotificationset-post
  description: Acknowledges notifications that were received from Enterprises.PullNotificationSet
    to prevent subsequent calls from returning the same notifications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/google-play/enterprisesacknowledgenotificationset-post-openapi.md
- name: Google Play - Get Notification Set
  x-api-slug: enterprisespullnotificationset-post
  description: |-
    Pulls and returns a notification set for the enterprises associated with the service account authenticated for the request. The notification set may be empty if no notification are pending.
    A notification set returned needs to be acknowledged within 20 seconds by calling Enterprises.AcknowledgeNotificationSet, unless the notification set is empty.
    Notifications that are not acknowledged within the 20 seconds will eventually be included again in the response to another PullNotificationSet request, and those that are never acknowledged will ultimately be deleted according to the Google Cloud Platform Pub/Sub system policy.
    Multiple requests might be performed concurrently to retrieve notifications, in which case the pending notifications (if any) will be split among each caller, if any are pending.
    If no notifications are present, an empty notification list is returned. Subsequent requests may return more notifications once they become available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/google-play/enterprisespullnotificationset-post-openapi.md
- name: Google Play - Create Acknowledges Notification Set
  x-api-slug: enterprisesacknowledgenotificationset-post
  description: Acknowledges notifications that were received from Enterprises.PullNotificationSet
    to prevent subsequent calls from returning the same notifications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/google-play/enterprisesacknowledgenotificationset-post-openapi.md
- name: Google Play - Get Notification Set
  x-api-slug: enterprisespullnotificationset-post
  description: |-
    Pulls and returns a notification set for the enterprises associated with the service account authenticated for the request. The notification set may be empty if no notification are pending.
    A notification set returned needs to be acknowledged within 20 seconds by calling Enterprises.AcknowledgeNotificationSet, unless the notification set is empty.
    Notifications that are not acknowledged within the 20 seconds will eventually be included again in the response to another PullNotificationSet request, and those that are never acknowledged will ultimately be deleted according to the Google Cloud Platform Pub/Sub system policy.
    Multiple requests might be performed concurrently to retrieve notifications, in which case the pending notifications (if any) will be split among each caller, if any are pending.
    If no notifications are present, an empty notification list is returned. Subsequent requests may return more notifications once they become available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/notifications/master/_listings/google-play/enterprisespullnotificationset-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.people.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.play.stack.network
- type: x-blog
  url: https://blog.google/products/google-play/
- type: x-blog-rss
  url: https://blog.google/products/google-play/rss
- type: x-developer
  url: https://developers.google.com/android-publisher/
- type: x-facebook
  url: https://www.facebook.com/GooglePlay
- type: x-getting-started
  url: https://developers.google.com/android-publisher/getting_started
- type: x-twitter
  url: https://twitter.com/GooglePlay
- type: x-website
  url: https://play.google.com/store
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---