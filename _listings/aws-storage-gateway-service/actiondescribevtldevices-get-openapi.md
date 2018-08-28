---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Describe VTL Devices
  version: 1.0.0
  description: |-
    Returns a description of virtual tape library (VTL) devices for the specified
             gateway.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeVTLDevices:
    get:
      summary: Describe VTL Devices
      description: |-
        Returns a description of virtual tape library (VTL) devices for the specified
                 gateway.
      operationId: describeVTLDevices
      x-api-path-slug: actiondescribevtldevices-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: Limit
        description: Specifies that the number of VTL devices described be limited
          to the specified         number
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          describing the VTL         devices
        type: string
      - in: query
        name: VTLDeviceARNs
        description: An array of strings, where each string represents the Amazon
          Resource Name (ARN) of a         VTL device
        type: string
      responses:
        200:
          description: OK
      tags:
      - VTL Devices
  /?Action=UpdateVTLDeviceType:
    get:
      summary: Update VTL Device Type
      description: Updates the type of medium changer in a gateway-VTL.
      operationId: updateVTLDeviceType
      x-api-path-slug: actionupdatevtldevicetype-get
      parameters:
      - in: query
        name: DeviceType
        description: The type of medium changer you want to select
        type: string
      - in: query
        name: VTLDeviceARN
        description: The Amazon Resource Name (ARN) of the medium changer you want
          to select
        type: string
      responses:
        200:
          description: OK
      tags:
      - VTL Device Type
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