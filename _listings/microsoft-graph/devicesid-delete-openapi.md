---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Delete Device
  description: Delete device Delete a registered device.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices:
    get:
      summary: List Devices
      description: List devices Retrieve a list of device objects registered in the
        organization.
      operationId: ListDevices
      x-api-path-slug: devices-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Devices
  /users/{id | userPrincipalName}/ownedDevices:
    get:
      summary: List Owned Devices
      description: List ownedDevices Get the list of devices that are owned by the
        user.
      operationId: ListOwnedDevices
      x-api-path-slug: usersid--userprincipalnameowneddevices-get
      parameters:
      - in: header
        name: Accept
        description: application/json
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Owned
      - Devices
  /users/{id | userPrincipalName}/registeredDevices:
    get:
      summary: List Registered Devices
      description: List registeredDevices Get the list of user's registered devices.
      operationId: ListRegisteredDevices
      x-api-path-slug: usersid--userprincipalnameregistereddevices-get
      parameters:
      - in: header
        name: Accept
        description: application/json
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Devices
  /devices/{id}:
    delete:
      summary: Delete Device
      description: Delete device Delete a registered device.
      operationId: DeleteDevice
      x-api-path-slug: devicesid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device
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