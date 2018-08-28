swagger: "2.0"
x-collection-name: Azure Storage
x-complete: 1
info:
  title: StorSimpleSeries8000ManagementClient
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/configureDevice
  : post:
      summary: Devices Configure
      description: Complete minimal setup before using the device.
      operationId: Devices_Configure
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernameconfiguredevice-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The minimal properties to configure a device
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Devices
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/devices:
    get:
      summary: Devices List By Manager
      description: Returns the list of devices for the specified manager.
      operationId: Devices_ListByManager
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevices-get
      parameters:
      - in: query
        name: $expand
        description: Specify $expand=details to populate additional fields related
          to the device
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Devices
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/devices/{deviceName}
  : get:
      summary: Devices Get
      description: Returns the properties of the specified device.
      operationId: Devices_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevicesdevicename-get
      parameters:
      - in: query
        name: $expand
        description: Specify $expand=details to populate additional fields related
          to the device
      - in: path
        name: deviceName
        description: The device name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Devices
    delete:
      summary: Devices Delete
      description: Deletes the device.
      operationId: Devices_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevicesdevicename-delete
      parameters:
      - in: path
        name: deviceName
        description: The device name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Devices
    patch:
      summary: Devices Update
      description: Patches the device.
      operationId: Devices_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevicesdevicename-patch
      parameters:
      - in: path
        name: deviceName
        description: The device Name
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Patch representation of the device
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Devices
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/devices/{deviceName}/deactivate
  : post:
      summary: Devices Deactivate
      description: Deactivates the device.
      operationId: Devices_Deactivate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevicesdevicenamedeactivate-post
      parameters:
      - in: path
        name: deviceName
        description: The device name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Devices