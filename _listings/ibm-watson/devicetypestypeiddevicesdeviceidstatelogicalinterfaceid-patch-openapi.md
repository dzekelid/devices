---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 0
info:
  title: IBM Watson IoT Platform Perform an operation against the device state for
    a logical interface
  description: |-
    Performs the specified operation against the device state for a logical
    interface. The following values can be specified for the operation
    property:

      - reset-state

    The **reset-state** operation will reset the state of the specified
    device to the default values as defined by the schema for the logical
    interface.
  version: 1.0.0
basePath: /api/v0002
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /device/types/{typeId}/devices/{deviceId}/state/{logicalInterfaceId}:
    get:
      summary: Get the state for the device with the specified id
      description: Retrieve the current state of the device with the specified id.
      operationId: retrieve-the-current-state-of-the-device-with-the-specified-id
      x-api-path-slug: devicetypestypeiddevicesdeviceidstatelogicalinterfaceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Device
      - Types
      - Devices
      - DeviceId
      - State
      - LogicalInterfaceId
    patch:
      summary: Perform an operation against the device state for a logical interface
      description: |-
        Performs the specified operation against the device state for a logical
        interface. The following values can be specified for the operation
        property:

          - reset-state

        The **reset-state** operation will reset the state of the specified
        device to the default values as defined by the schema for the logical
        interface.
      operationId: performs-the-specified-operation-against-the-device-state-for-a-logicalinterface-the-following-value
      x-api-path-slug: devicetypestypeiddevicesdeviceidstatelogicalinterfaceid-patch
      parameters:
      - in: query
        name: No Name
      - in: body
        name: Operation
        description: The JSON representation of an operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Device
      - Types
      - Devices
      - DeviceId
      - State
      - LogicalInterfaceId
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