---
name: Fitbit
x-slug: fitbit
description: Find your fit with Fitbits family of fitness products that help you stay
  motivated and improve your health by tracking your activity, exercise, food, weight
  and sleep.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/200-fitbit.jpg
x-kinRank: "9"
x-alexaRank: "2266"
tags: Devices
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/fitbit/apis.md
specificationVersion: "0.14"
apis:
- name: Fitbit Get User Devices.json
  x-api-slug: fitbit
  description: Retrieve the list of Fitbit devices for a user in the format requested.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/200-fitbit.jpg
  humanURL: http://fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/devices.json
  tags: User,-,Devices.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/fitbit/userdevices-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/fitbit/userdevices-json-get-openapi.md
- name: Fitbit
  x-api-slug: fitbit
  description: Find your fit with Fitbits family of fitness products that help you
    stay motivated and improve your health by tracking your activity, exercise, food,
    weight and sleep.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/200-fitbit.jpg
  humanURL: http://fitbit.com
  baseURL: https://api.fitbit.com//1
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/fitbit/openapi.md
x-common:
- type: x-api-json--authoritative
  url: https://www.fitbit.com/apis.json
- type: x-apigee-console
  url: https://wiki.fitbit.com/display/API/API+Explorer
- type: x-blog
  url: http://blog.fitbit.com
- type: x-blog-rss
  url: http://blog.fitbit.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/fitbit
- type: x-crunchbase
  url: https://crunchbase.com/organization/fitbit
- type: x-email
  url: privacy@fitbit.com
- type: x-github
  url: https://github.com/fitbit
- type: x-rate-limits
  url: https://wiki.fitbit.com/display/API/Rate+Limit
- type: x-twitter
  url: https://twitter.com/fitbit
- type: x-website
  url: http://fitbit.com
- type: x-website
  url: http://dev.fitbit.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---