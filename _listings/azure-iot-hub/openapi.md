---
swagger: "2.0"
x-collection-name: Azure IoT Hub
x-complete: 1
info:
  title: iotHubClient
  description: use-this-api-to-manage-the-iot-hubs-in-your-subscription-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/IotHubs/{resourceName}/exportDevices
  : post:
      summary: Iot Hub Resource Export Devices
      description: 'Exports all the device identities in the IoT hub identity registry
        to an Azure Storage blob container. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry#import-and-export-device-identities.'
      operationId: IotHubResource_ExportDevices
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devicesiothubsresourcenameexportdevices-post
      parameters:
      - in: body
        name: exportDevicesParameters
        description: The parameters that specify the export devices operation
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group that contains the IoT hub
      - in: path
        name: resourceName
        description: The name of the IoT hub
      responses:
        200:
          description: OK
      tags:
      - Iot Hub Resource Export Devices
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/IotHubs/{resourceName}/importDevices
  : post:
      summary: Iot Hub Resource Import Devices
      description: 'Import, update, or delete device identities in the IoT hub identity
        registry from a blob. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry#import-and-export-device-identities.'
      operationId: IotHubResource_ImportDevices
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devicesiothubsresourcenameimportdevices-post
      parameters:
      - in: body
        name: importDevicesParameters
        description: The parameters that specify the import devices operation
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group that contains the IoT hub
      - in: path
        name: resourceName
        description: The name of the IoT hub
      responses:
        200:
          description: OK
      tags:
      - Iot Hub Resource Import Devices
---