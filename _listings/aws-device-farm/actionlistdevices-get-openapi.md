---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 0
info:
  title: AWS Device Farm API List Devices
  version: 1.0.0
  description: Gets information about unique device types.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetDevice:
    get:
      summary: Get Device
      description: Gets information about a unique device type.
      operationId: getDevice
      x-api-path-slug: actiongetdevice-get
      parameters:
      - in: query
        name: arn
        description: The device types ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=ListDevices:
    get:
      summary: List Devices
      description: Gets information about unique device types.
      operationId: listDevices
      x-api-path-slug: actionlistdevices-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the project
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=CreateDevicePool:
    get:
      summary: Create Device Pool
      description: Creates a device pool.
      operationId: createDevicePool
      x-api-path-slug: actioncreatedevicepool-get
      parameters:
      - in: query
        name: description
        description: The device pools description
        type: string
      - in: query
        name: name
        description: The device pools name
        type: string
      - in: query
        name: projectArn
        description: The ARN of the project for the device pool
        type: string
      - in: query
        name: rules
        description: The device pools rules
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
  /?Action=DeleteDevicePool:
    get:
      summary: Delete Device Pool
      description: Deletes a device pool given the pool ARN.
      operationId: deleteDevicePool
      x-api-path-slug: actiondeletedevicepool-get
      parameters:
      - in: query
        name: arn
        description: Represents the Amazon Resource Name (ARN) of the Device Farm
          device pool you wish to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
  /?Action=DeleteProject:
    get:
      summary: Delete Project
      description: Deletes an AWS Device Farm project, given the project ARN.
      operationId: deleteProject
      x-api-path-slug: actiondeleteproject-get
      parameters:
      - in: query
        name: arn
        description: Represents the Amazon Resource Name (ARN) of the Device Farm
          project you wish to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Projects
  /?Action=GetDevicePool:
    get:
      summary: Get Device Pool
      description: Gets information about a device pool.
      operationId: getDevicePool
      x-api-path-slug: actiongetdevicepool-get
      parameters:
      - in: query
        name: arn
        description: The device pools ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
  /?Action=GetDevicePoolCompatibility:
    get:
      summary: Get Device Pool Compatibility
      description: Gets information about compatibility with a device pool.
      operationId: getDevicePoolCompatibility
      x-api-path-slug: actiongetdevicepoolcompatibility-get
      parameters:
      - in: query
        name: appArn
        description: The ARN of the app that is associated with the specified device
          pool
        type: string
      - in: query
        name: devicePoolArn
        description: The device pools ARN
        type: string
      - in: query
        name: testType
        description: The test type for the specified device pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
  /?Action=ListDevicePools:
    get:
      summary: List Device Pools
      description: Gets information about device pools.
      operationId: listDevicePools
      x-api-path-slug: actionlistdevicepools-get
      parameters:
      - in: query
        name: arn
        description: The project ARN
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      - in: query
        name: type
        description: The device pools type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
  /?Action=ListRuns:
    get:
      summary: List Runs
      description: Gets information about runs, given an AWS Device Farm project ARN.
      operationId: listRuns
      x-api-path-slug: actionlistruns-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the project for which you want
          to list runs
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
  /?Action=ListSamples:
    get:
      summary: List Samples
      description: Gets information about samples, given an AWS Device Farm project
        ARN.
      operationId: listSamples
      x-api-path-slug: actionlistsamples-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the project for which you want
          to list samples
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Samples
  /?Action=ListUploads:
    get:
      summary: List Uploads
      description: Gets information about uploads, given an AWS Device Farm project
        ARN.
      operationId: listUploads
      x-api-path-slug: actionlistuploads-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the project for which you want
          to list uploads
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Uploads
  /?Action=UpdateDevicePool:
    get:
      summary: Update Device Pool
      description: Modifies the name, description, and rules in a device pool given
        the attributes and the pool ARN.
      operationId: updateDevicePool
      x-api-path-slug: actionupdatedevicepool-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resourc Name (ARN) of the Device Farm device pool
          you wish to update
        type: string
      - in: query
        name: description
        description: A description of the device pool you wish to update
        type: string
      - in: query
        name: name
        description: A string representing the name of the device pool you wish to
          update
        type: string
      - in: query
        name: rules
        description: Represents the rules you wish to modify for the device pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
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