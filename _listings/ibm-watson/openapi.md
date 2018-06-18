---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 1
info:
  title: IBM Watson IoT Platform HTTP REST API
  description: the-information-management-capabilities-of-ibm-watson-iot-platform-helpyou-to-organize-and-integrate-data-coming-in-to-and-going-out-of-watson-iotplatform---with-these-apis-you-will-be-able-to---work-with-device-state-regardless-of-whether-the-actual-device-on-online----or-offline----provide-your-application-developers-with-consistent-interfaces-to-access----eventdriven-device-data-in-a-restlike-manner----normalize-data-from-devices-of-different-makes-or-models-that-publish----data-in-different-formatsfor-information-on-how-to-use-watson-iot-platform-apis-generally-see-the-api-documentationhttpsconsole-ng-bluemix-netdocsservicesiotreferenceapi-html-for-more-general-information-on-how-to-use-watson-iot-platform-seethe-general-documentationhttpsconsole-ng-bluemix-netdocsservicesiotindex-htmlgettingstartedtemplate
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
---