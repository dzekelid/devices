---
name: Clover
x-slug: clover
description: Clover, a First Data company, builds the largest open-architecture point
  of sale solution aimed at small &amp; medium sized business owners. Our products
  are changing the consumer/merchant experience for the better, opening avenues for
  seamless customer-merchant interactions. There are five versions of Clover, including
  the Clover Station, Clover Mobile, Clover Mini, Clover Go, and Clover Flex. With
  Clover, First Data is aiming to create the largest open architecture operating system
  for commerce-enabling solutions and applications for business owners.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
x-kinRank: "7"
x-alexaRank: "23096"
tags: Devices
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/clover/apis.md
specificationVersion: "0.14"
apis:
- name: ' - Get all devices provisioned to a merchant'
  x-api-slug: v3merchantsmiddevices-get
  description: Returns a list of all devices that are provisioned to the a merchant.
    This list can be viewed from the Setup App on the merchant's device or web dashboard
    (https://www.clover.com/setupapp/m/{mId}/devices).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/clover/v3merchantsmiddevices-get-openapi.md
- name: ' - Get a single device provisioned to a merchant'
  x-api-slug: v3merchantsmiddevicesdeviceid-get
  description: Returns a single device that is provisioned to a merchant.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/clover/v3merchantsmiddevicesdeviceid-get-openapi.md
- name: ' - Get all cash events for a device'
  x-api-slug: v3merchantsmiddevicesdeviceidcash-events-get
  description: Retrieve cash events filtered by device ID. Cash events can also be
    consumed by registering a Webhook callback. See https://docs.clover.com/build/webhooks/
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/clover/v3merchantsmiddevicesdeviceidcash-events-get-openapi.md
- name: ' - Create a notification for a device'
  x-api-slug: v3appsaiddevicesdidnotifications-post
  description: 'Push a message to a device that has your app installed and is listening
    for notifications.  For details on how to use Clover''s Android SDK to receive
    notifications see: https://github.com/clover/android-examples/tree/master/pushnotificationexample'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/clover/v3appsaiddevicesdidnotifications-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://cloudflare.api.gallery.streamdata.io
- type: x-api-stack
  url: http://clover.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/clover
- type: x-developer
  url: https://www.clover.com/developers
- type: x-documentation
  url: https://docs.clover.com/
- type: x-github
  url: https://github.com/clover
- type: x-twitter
  url: https://twitter.com/CloverPOS
- type: x-website
  url: https://www.clover.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---