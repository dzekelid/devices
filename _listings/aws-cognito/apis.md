---
name: AWS Cognito
x-slug: aws-cognito
description: Amazon Cognito lets you easily add user sign-up and sign-in to your mobile
  and web apps. With Amazon Cognito, you also have the options to authenticate users
  through social identity providers such as Facebook, Twitter, or Amazon, with SAML
  identity solutions, or by using your own identity system. In addition, Amazon Cognito
  enables you to save data locally on users devices, allowing your applications to
  work even when the devices are offline. You can then synchronize data across users
  devices so that their app experience remains consistent regardless of the device
  they use. With Amazon Cognito, you can focus on creating great app experiences instead
  of worrying about building, securing, and scaling a solution to handle user management,
  authentication, and sync across devices.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Devices
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Cognito API Admin Forget Device
  x-api-slug: aws-cognito-api
  description: Forgets the device, as an administrator.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminForgetDevice
  tags: Devices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionadminforgetdevice-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionadminforgetdevice-get-openapi.md
- name: AWS Cognito API Confirm Device
  x-api-slug: aws-cognito-api
  description: Confirms tracking of the device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=ConfirmDevice
  tags: Devices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionconfirmdevice-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionconfirmdevice-get-openapi.md
- name: AWS Cognito API Forget Device
  x-api-slug: aws-cognito-api
  description: Forgets the specified device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=ForgetDevice
  tags: Devices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionforgetdevice-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionforgetdevice-get-openapi.md
- name: AWS Cognito API List Devices
  x-api-slug: aws-cognito-api
  description: Lists the devices.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=ListDevices
  tags: Devices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionlistdevices-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionlistdevices-get-openapi.md
- name: AWS Cognito API Update Device Status
  x-api-slug: aws-cognito-api
  description: Updates the device status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=UpdateDeviceStatus
  tags: Devices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionupdatedevicestatus-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionupdatedevicestatus-get-openapi.md
- name: AWS Cognito API Register Device
  x-api-slug: aws-cognito-api
  description: Registers a device to receive push sync notifications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=RegisterDevice
  tags: Devices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionregisterdevice-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/actionregisterdevice-get-openapi.md
- name: AWS Cognito API
  x-api-slug: aws-cognito-api
  description: Amazon Cognito lets you easily add user sign-up and sign-in to your
    mobile and web apps. With Amazon Cognito, you also have the options to authenticate
    users through social identity providers such as Facebook, Twitter, or Amazon,
    with SAML identity solutions, or by using your own identity system. In addition,
    Amazon Cognito enables you to save data locally on users devices, allowing your
    applications to work even when the devices are offline. You can then synchronize
    data across users devices so that their app experience remains consistent regardless
    of the device they use. With Amazon Cognito, you can focus on creating great app
    experiences instead of worrying about building, securing, and scaling a solution
    to handle user management, authentication, and sync across devices.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https:///
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-cognito/openapi.md
x-common:
- type: x-blog
  url: https://aws.amazon.com/cognito/dev-resources/#blogposts
- type: x-documentation
  url: http://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/Welcome.html
- type: x-documentation
  url: http://docs.aws.amazon.com/cognitoidentity/latest/APIReference/Welcome.html
- type: x-documentation
  url: http://docs.aws.amazon.com/cognitosync/latest/APIReference/Welcome.html
- type: x-faq
  url: http://aws.amazon.com/cognito/faqs
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=173
- type: x-pricing
  url: http://aws.amazon.com/cognito/pricing
- type: x-sdk
  url: https://aws.amazon.com/cognito/dev-resources/#documentation
- type: x-slides
  url: https://aws.amazon.com/cognito/dev-resources/#slides
- type: x-videos
  url: https://aws.amazon.com/cognito/dev-resources/#videos
- type: x-website
  url: https://aws.amazon.com/cognito/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---