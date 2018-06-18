---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 1
info:
  title: AWS Device Farm API
  version: 1.0.0
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
---