---
name: Azure Storage
x-slug: azure-storage
description: Azure Storage offers non-relational data storage including Blob Storage,
  Table Storage, Queue Storage, and Files.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-storage.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Devices
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-storage/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Storage API Devices Configure
  x-api-slug: azure-storage-api
  description: Complete minimal setup before using the device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-storage.png
  humanURL: https://azure.microsoft.com/en-us/services/storage/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/configureDevice
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-storage/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernameconfiguredevice-post-openapi.md
- name: Azure Storage API Devices List By Manager
  x-api-slug: azure-storage-api
  description: Returns the list of devices for the specified manager.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-storage.png
  humanURL: https://azure.microsoft.com/en-us/services/storage/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/devices
  tags: Devices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-storage/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevices-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-storage/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevices-get-openapi.md
- name: Azure Storage API Devices Get
  x-api-slug: azure-storage-api
  description: Returns the properties of the specified device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-storage.png
  humanURL: https://azure.microsoft.com/en-us/services/storage/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/devices/{deviceName}
  tags: Devices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-storage/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevicesdevicename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-storage/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevicesdevicename-get-openapi.md
- name: Azure Storage API Devices Delete
  x-api-slug: azure-storage-api
  description: Deletes the device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-storage.png
  humanURL: https://azure.microsoft.com/en-us/services/storage/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/devices/{deviceName}
  tags: Devices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-storage/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevicesdevicename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-storage/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevicesdevicename-delete-openapi.md
- name: Azure Storage API Devices Update
  x-api-slug: azure-storage-api
  description: Patches the device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-storage.png
  humanURL: https://azure.microsoft.com/en-us/services/storage/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/devices/{deviceName}
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-storage/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevicesdevicename-patch-openapi.md
- name: Azure Storage API Devices Deactivate
  x-api-slug: azure-storage-api
  description: Deactivates the device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-storage.png
  humanURL: https://azure.microsoft.com/en-us/services/storage/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/devices/{deviceName}/deactivate
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-storage/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevicesdevicenamedeactivate-post-openapi.md
- name: Azure Storage API
  x-api-slug: azure-storage-api
  description: Azure Storage offers non-relational data storage including Blob Storage,
    Table Storage, Queue Storage, and Files.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-storage.png
  humanURL: https://azure.microsoft.com/en-us/services/storage/
  baseURL: ://management.azure.com//
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-storage/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/storage/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/storage/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/storage/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/storage/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---