---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
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
---