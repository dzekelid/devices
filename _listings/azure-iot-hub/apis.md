---
name: Azure IoT Hub
x-slug: azure-iot-hub
description: Jumpstart your Internet of Things project with Microsoft IoT Hub. Connect,
  monitor, and control billions of IoT assets running on a broad set of operating
  systems and protocols. Establish reliable, bi-directional communication with these
  assets, even if they&rsquo;re intermittently connected, and analyze&mdash;and act
  on&mdash;incoming telemetry data. Enhance the security of your IoT solutions by
  using per-device authentication to communicate with devices that have the appropriate
  credentials. Revoke access rights to specific devices to maintain the integrity
  of your system.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-iot-01-establish.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Devices
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-iot-hub/apis.md
specificationVersion: "0.14"
apis:
- name: Azure IoT Hub API Iot Hub Resource Export Devices
  x-api-slug: azure-iot-hub-api
  description: 'Exports all the device identities in the IoT hub identity registry
    to an Azure Storage blob container. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry#import-and-export-device-identities.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-iot-01-establish.png
  humanURL: https://azure.microsoft.com/en-us/services/iot-hub/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/IotHubs/{resourceName}/exportDevices
  tags: Iot Hub Resource Export Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-iot-hub/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devicesiothubsresourcenameexportdevices-post-openapi.md
- name: Azure IoT Hub API Iot Hub Resource Import Devices
  x-api-slug: azure-iot-hub-api
  description: 'Import, update, or delete device identities in the IoT hub identity
    registry from a blob. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry#import-and-export-device-identities.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-iot-01-establish.png
  humanURL: https://azure.microsoft.com/en-us/services/iot-hub/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/IotHubs/{resourceName}/importDevices
  tags: Iot Hub Resource Import Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-iot-hub/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devicesiothubsresourcenameimportdevices-post-openapi.md
- name: Azure IoT Hub API
  x-api-slug: azure-iot-hub-api
  description: Jumpstart your Internet of Things project with Microsoft IoT Hub. Connect,
    monitor, and control billions of IoT assets running on a broad set of operating
    systems and protocols. Establish reliable, bi-directional communication with these
    assets, even if they&rsquo;re intermittently connected, and analyze&mdash;and
    act on&mdash;incoming telemetry data. Enhance the security of your IoT solutions
    by using per-device authentication to communicate with devices that have the appropriate
    credentials. Revoke access rights to specific devices to maintain the integrity
    of your system.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-iot-01-establish.png
  humanURL: https://azure.microsoft.com/en-us/services/iot-hub/
  baseURL: ://management.azure.com//
  tags: Devices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/azure-iot-hub/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/iot-hub/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/iot-hub/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/iot-hub/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/iot-hub/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---