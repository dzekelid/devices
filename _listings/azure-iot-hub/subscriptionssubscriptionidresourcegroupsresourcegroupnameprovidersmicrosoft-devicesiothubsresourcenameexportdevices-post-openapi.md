---
swagger: "2.0"
x-collection-name: Azure IoT Hub
x-complete: 0
info:
  title: Azure IoT Hub API Iot Hub Resource Export Devices
  description: 'Exports all the device identities in the IoT hub identity registry
    to an Azure Storage blob container. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry#import-and-export-device-identities.'
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---