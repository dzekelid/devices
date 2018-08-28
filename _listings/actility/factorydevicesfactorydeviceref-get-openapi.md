---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Maker API Factory device retrieval
  description: Retrieves the factory device corresponding to the provided factoryDeviceRef.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices:
    get:
      summary: Devices retrieval
      description: 'Retrieves a list of devices existing within authorized scopes.
        Note that for each device, by default only the following information is retrieved:
        ''ref'', ''name'', ''EUI'', ''networkAddress''.'
      operationId: retrieves-a-list-of-devices-existing-within-authorized-scopes-note-that-for-each-device-by-default-o
      x-api-path-slug: devices-get
      parameters:
      - in: query
        name: commercialDetails
        description: Indicates to also retrieve commercial information along each
          device
      - in: query
        name: connectivityPlanId
        description: Connectivity plan assigned to the devices to search for
      - in: query
        name: deviceEUI
        description: EUI of the device to search for
      - in: query
        name: deviceToken
        description: Token provided by the manufacturer for an easy registration on
          a standalone Join Server
      - in: query
        name: extendedInfo
        description: Indicates to retrieve all available information (including statistics
          and commercial details) along each device
      - in: query
        name: healthState
        description: Health state of the devices to search for
      - in: query
        name: pageIndex
        description: If set, enables pagination and returns only the 100 devices of
          the specified page
      - in: query
        name: statistics
        description: Indicates to also retrieve usage statistic information along
          each device
      responses:
        200:
          description: OK
      tags:
      - Devices
      - Retrieval
    post:
      summary: Device creation
      description: Creates a new device. If no 'routingProfileId' or 'processingStrategyId'
        values are provided, then 'processingStrategyId' will be automatically set
        to 'DATAFLOW'. If no 'connectivityPlanId' value is provided, then the first
        connectivity plan of the subscriber with available connections will be assigned
        to the device.
      operationId: creates-a-new-device-if-no-routingprofileid-or-processingstrategyid-values-are-provided-then-process
      x-api-path-slug: devices-post
      parameters:
      - in: body
        name: device
        description: Contents of the device to create
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: deviceToken
        description: Token provided by the manufacturer for an easy registration on
          a standalone Join Server
      responses:
        200:
          description: OK
      tags:
      - Device
      - Creation
  /devices/{deviceRef}:
    get:
      summary: Device retrieval
      description: Retrieves the device corresponding to the provided device ref,
        if that device is within authorized scopes.
      operationId: retrieves-the-device-corresponding-to-the-provided-device-ref-if-that-device-is-within-authorized-sc
      x-api-path-slug: devicesdeviceref-get
      parameters:
      - in: path
        name: deviceRef
        description: Ref of the device to retrieve
      responses:
        200:
          description: OK
      tags:
      - Device
      - Retrieval
    put:
      summary: Device update
      description: 'Updates the device corresponding to the provided device ref, if
        that device is within authorized scopes. Only following attributes can be
        updated: ''name'', ''routingProfileId'', ''processingStrategyId'', ''connectivityPlanId'',
        ''deviceProfileId'' and ''applicationEUI''. To update other attributes, device
        must be deleted than re-created.'
      operationId: updates-the-device-corresponding-to-the-provided-device-ref-if-that-device-is-within-authorized-scop
      x-api-path-slug: devicesdeviceref-put
      parameters:
      - in: body
        name: device
        description: Contents of the device to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: deviceRef
        description: Ref of the device to update
      - in: query
        name: deviceToken
        description: Token provided by the manufacturer for an easy registration on
          a standalone Join Server
      responses:
        200:
          description: OK
      tags:
      - Device
      - Update
    delete:
      summary: Device deletion
      description: Deletes the device corresponding to the provided device ref, if
        that device is within authorized scopes.
      operationId: deletes-the-device-corresponding-to-the-provided-device-ref-if-that-device-is-within-authorized-scop
      x-api-path-slug: devicesdeviceref-delete
      parameters:
      - in: path
        name: deviceRef
        description: Ref of the device to delete
      responses:
        200:
          description: OK
      tags:
      - Device
      - Deletion
  /deviceProfiles:
    get:
      summary: Device profiles retrieval
      description: Retrieves the list of existing device profiles.
      operationId: retrieves-the-list-of-existing-device-profiles
      x-api-path-slug: deviceprofiles-get
      responses:
        200:
          description: OK
      tags:
      - Device
      - Profiles
      - Retrieval
  /deviceAlarms:
    get:
      summary: Device alarms retrieval
      description: Retrieves a list of device alarms existing within authorized scopes.
      operationId: retrieves-a-list-of-device-alarms-existing-within-authorized-scopes
      x-api-path-slug: devicealarms-get
      parameters:
      - in: query
        name: deviceEUI
        description: EUI of the device to search alarms for
      - in: query
        name: pageIndex
        description: If set, enables pagination and returns only the 100 device alarms
          of the specified page
      responses:
        200:
          description: OK
      tags:
      - Device
      - Alarms
      - Retrieval
  /deviceAlarms/{deviceAlarmRef}:
    get:
      summary: Device alarm retrieval
      description: Retrieves the device alarm corresponding to the provided device
        alarm ref, if that device alarm is within authorized scopes.
      operationId: retrieves-the-device-alarm-corresponding-to-the-provided-device-alarm-ref-if-that-device-alarm-is-wi
      x-api-path-slug: devicealarmsdevicealarmref-get
      parameters:
      - in: path
        name: deviceAlarmRef
        description: Ref of the device alarm to retrieve
      responses:
        200:
          description: OK
      tags:
      - Device
      - Alarm
      - Retrieval
  /deviceAlarms/{deviceAlarmRef}/acks:
    post:
      summary: Device alarm acknowledgement
      description: Acknowledges a device alarm.
      operationId: acknowledges-a-device-alarm
      x-api-path-slug: devicealarmsdevicealarmrefacks-post
      parameters:
      - in: path
        name: deviceAlarmRef
        description: Ref of the device alarm to acknowledge
      responses:
        200:
          description: OK
      tags:
      - Device
      - Alarm
      - Acknowledgement
  /factoryDevices:
    get:
      summary: Factory devices retrieval
      description: Retrieves all factory devices.
      operationId: retrieves-all-factory-devices
      x-api-path-slug: factorydevices-get
      parameters:
      - in: query
        name: deviceEUI
        description: EUI of the factory device to retrieve
      - in: query
        name: pageIndex
        description: If set, enables pagination and returns only the 100 factory devices
          of the specified page
      responses:
        200:
          description: OK
      tags:
      - Factory
      - Devices
      - Retrieval
    post:
      summary: Factory device creation
      description: Creates a factory device.
      operationId: creates-a-factory-device
      x-api-path-slug: factorydevices-post
      parameters:
      - in: body
        name: deviceFactory
        description: Contents of the factory device
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Factory
      - Device
      - Creation
  /factoryDevices/{factoryDeviceRef}:
    get:
      summary: Factory device retrieval
      description: Retrieves the factory device corresponding to the provided factoryDeviceRef.
      operationId: retrieves-the-factory-device-corresponding-to-the-provided-factorydeviceref
      x-api-path-slug: factorydevicesfactorydeviceref-get
      parameters:
      - in: path
        name: factoryDeviceRef
        description: Ref of the factory device to retrieve
      responses:
        200:
          description: OK
      tags:
      - Factory
      - Device
      - Retrieval
    put:
      summary: Factory device update
      description: Updates the factory device corresponding to the provided factoryDeviceRef.
      operationId: updates-the-factory-device-corresponding-to-the-provided-factorydeviceref
      x-api-path-slug: factorydevicesfactorydeviceref-put
      parameters:
      - in: body
        name: device
        description: Contents of the factory device to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: factoryDeviceRef
        description: Ref of the factory device to update
      responses:
        200:
          description: OK
      tags:
      - Factory
      - Device
      - Update
    delete:
      summary: Factory device deletion
      description: Deletes the factory device corresponding to the provided factoryDeviceRef.
      operationId: deletes-the-factory-device-corresponding-to-the-provided-factorydeviceref
      x-api-path-slug: factorydevicesfactorydeviceref-delete
      parameters:
      - in: path
        name: factoryDeviceRef
        description: Ref of the factory device to delete
      responses:
        200:
          description: OK
      tags:
      - Factory
      - Device
      - Deletion
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