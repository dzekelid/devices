---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 0
info:
  title: IBM Watson IoT Platform Get the list of active property mappings for the
    device type
  description: |-
    Retrieve the list of active property mappings for the specified device
    type.  A property mapping defines how properties from inbound events are
    mapped to properties defined on an logical interface associated with
    the device type.
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
  /device/types:
    get:
      summary: List device types
      description: |-
        Sorting can be performed on any of the following properties (sort
        order can be reversed by prefixing the property name with '-'):
        - id
        - description
        - deviceInfo.description
        - deviceInfo.descriptiveLocation
        - deviceInfo.serialNumber
        - deviceInfo.deviceClass
        - deviceInfo.fwVersion
        - deviceInfo.hwVersion
        - deviceInfo.manufacturer
        - deviceInfo.model

        The following facets are supported:
        - deviceInfo.deviceClass
        - deviceInfo.fwVersion
        - deviceInfo.hwVersion
        - deviceInfo.manufacturer
        - deviceInfo.model
      operationId: sorting-can-be-performed-on-any-of-the-following-properties-sortorder-can-be-reversed-by-prefixing-t
      x-api-path-slug: devicetypes-get
      parameters:
      - in: query
        name: description
        description: Optional filter of results by description
      - in: query
        name: id
        description: Optional filter of results by ID
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Device
      - Types
  /device/types/{typeId}:
    patch:
      summary: Perform an operation against a device type
      description: |-
        Performs the specified operation against the device type. The following
        values can be specified for the operation property:

          - deactivate-configuration

        The **deactivate-configuration** operation will remove any activate
        configuration that is currently associated with the device type. If any
        instances of the device type exist, the state for those devices will be
        deleted as a result of performing the **deactivate-configuration**
        operation. The **deactivate-configuration** operation will fail if
        any instances of the device type are being aggregated into an instance
        of a thing.
      operationId: performs-the-specified-operation-against-the-device-type-the-followingvalues-can-be-specified-for-th
      x-api-path-slug: devicetypestypeid-patch
      parameters:
      - in: body
        name: Device Type Operation
        description: The JSON representation of a device type operation
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Device
      - Types
  /device/types/{typeId}/physicalinterface:
    get:
      summary: Get the active physical interface associated with the device type
      description: |-
        Retrieve the active physical interface that has been associated with the
        device type.  At least one active physical interface must be associated
        with the device type before any mappings can be defined that will
        generate state for the device.
      operationId: retrieve-the-active-physical-interface-that-has-been-associated-with-thedevice-type--at-least-one-ac
      x-api-path-slug: devicetypestypeidphysicalinterface-get
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
      - Physicalinterface
  /device/types/{typeId}/logicalinterfaces:
    get:
      summary: |-
        Get the list of active logical interfaces associated with the device
        type
      description: |-
        Retrieve the list of active logical interfaces that have been
        associated with the device type.  At least one logical interface
        must be associated with the device type before any mappings can be
        defined that will generate state for the device.
      operationId: retrieve-the-list-of-active-logical-interfaces-that-have-beenassociated-with-the-device-type--at-lea
      x-api-path-slug: devicetypestypeidlogicalinterfaces-get
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
      - Logical interfaces
  /device/types/{typeId}/mappings:
    get:
      summary: Get the list of active property mappings for the device type
      description: |-
        Retrieve the list of active property mappings for the specified device
        type.  A property mapping defines how properties from inbound events are
        mapped to properties defined on an logical interface associated with
        the device type.
      operationId: retrieve-the-list-of-active-property-mappings-for-the-specified-devicetype--a-property-mapping-defin
      x-api-path-slug: devicetypestypeidmappings-get
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
      - Mappings
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