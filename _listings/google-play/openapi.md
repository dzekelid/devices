swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /enterprises/{enterpriseId}/users/{userId}/devices:
    get:
      summary: Get User Devices
      description: Retrieves the IDs of all of a user's devices.
      operationId: androidenterprise.devices.list
      x-api-path-slug: enterprisesenterpriseidusersuseriddevices-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Device
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}:
    get:
      summary: Get User Device
      description: Retrieves the details of a device.
      operationId: androidenterprise.devices.get
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceid-get
      parameters:
      - in: path
        name: deviceId
        description: The ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Device