---
name: VictorOps
x-slug: victorops
description: VictorOps incident managament software gives DevOps observability, collaboration,
  & real-time alerting, to build, deploy, & operate software. Learn more.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
x-kinRank: "8"
x-alexaRank: "196587"
tags: Devices
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/victorops/apis.md
specificationVersion: "0.14"
apis:
- name: Victor Ops Get a list of all contact devices for a user
  x-api-slug: victor-ops
  description: |-
    Get the contact methods for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/devices
  tags: User,User,Contact-methods,Devices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/victorops/apipublicv1userusercontactmethodsdevices-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/victorops/apipublicv1userusercontactmethodsdevices-get-openapi.md
- name: Victor Ops Delete a contact device for a user
  x-api-slug: victor-ops
  description: |-
    Delete a contact device for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/devices/{contactId}
  tags: User,User,Contact-methods,Devices,ContactId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-delete-openapi.md
- name: Victor Ops Get the indicated contact device for a user
  x-api-slug: victor-ops
  description: |-
    Get the indicated contact device for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/devices/{contactId}
  tags: User,User,Contact-methods,Devices,ContactId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-get-openapi.md
- name: Victor Ops Update a contact device for a user
  x-api-slug: victor-ops
  description: |-
    Update a contact device for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/devices/{contactId}
  tags: User,User,Contact-methods,Devices,ContactId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-put-openapi.md
- name: Victor Ops
  x-api-slug: victor-ops
  description: VictorOps incident managament software gives DevOps observability,
    collaboration, & real-time alerting, to build, deploy, & operate software. Learn
    more.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com//
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/victorops/openapi.md
x-common:
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