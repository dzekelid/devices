---
name: AWS Identity and Access Management
x-slug: aws-identity-and-access-management
description: AWS Identity and Access Management (IAM) enables you to securely control
  access to AWS services and resources for your users. Using IAM, you can create and
  manage AWS users and groups, and use permissions to allow and deny their access
  to AWS resources.IAM is a feature of your AWS account offered at no additional charge.
  You will be charged only for use of other AWS services by your users.To get started
  using IAM, orif you have already registered with AWS, go to theAWS Management Consoleand
  get started with theseIAM Best Practices.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Devices
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-identity-and-access-management/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Identity and Access Management API Delete Virtual M F A Device
  x-api-slug: aws-identity-and-access-management-api
  description: Deletes a virtual MFA device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=DeleteVirtualMFADevice
  tags: Virtual MFA Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-identity-and-access-management/actiondeletevirtualmfadevice-get-openapi.md
- name: AWS Identity and Access Management API Enable M F A Device
  x-api-slug: aws-identity-and-access-management-api
  description: Enables the specified MFA device and associates it with the specified
    IAM user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=EnableMFADevice
  tags: MFA Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-identity-and-access-management/actionenablemfadevice-get-openapi.md
- name: AWS Identity and Access Management API List M F A Devices
  x-api-slug: aws-identity-and-access-management-api
  description: Lists the MFA devices for an IAM user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=ListMFADevices
  tags: MFA Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-identity-and-access-management/actionlistmfadevices-get-openapi.md
- name: AWS Identity and Access Management API List Virtual M F A Devices
  x-api-slug: aws-identity-and-access-management-api
  description: Lists the virtual MFA devices defined in the AWS account by assignment
    status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=ListVirtualMFADevices
  tags: Virtual MFA Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-identity-and-access-management/actionlistvirtualmfadevices-get-openapi.md
- name: AWS Identity and Access Management API Resync M F A Device
  x-api-slug: aws-identity-and-access-management-api
  description: |-
    Synchronizes the specified MFA device with its IAM resource object on the AWS
          servers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=ResyncMFADevice
  tags: MFA Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-identity-and-access-management/actionresyncmfadevice-get-openapi.md
- name: AWS Identity and Access Management API
  x-api-slug: aws-identity-and-access-management-api
  description: AWS Identity and Access Management (IAM) enables you to securely control
    access to AWS services and resources for your users. Using IAM, you can create
    and manage AWS users and groups, and use permissions to allow and deny their access
    to AWS resources.IAM is a feature of your AWS account offered at no additional
    charge. You will be charged only for use of other AWS services by your users.To
    get started using IAM, orif you have already registered with AWS, go to theAWS
    Management Consoleand get started with theseIAM Best Practices.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: :///
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/aws-identity-and-access-management/openapi.md
x-common:
- type: x-change-log
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=323
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/sts/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/IAM/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/iam/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=76
- type: x-getting-started
  url: https://aws.amazon.com/iam/getting-started/
- type: x-partners
  url: https://aws.amazon.com/iam/partners/
- type: x-tools
  url: http://aws.amazon.com/cli
- type: x-website
  url: https://aws.amazon.com/iam/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---