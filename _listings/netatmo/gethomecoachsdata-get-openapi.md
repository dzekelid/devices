---
swagger: "2.0"
x-collection-name: Netatmo
x-complete: 0
info:
  title: Netatmo Get Gethomecoachsdata
  description: The method gethomecoachsdata Returns data from a user Healthy Home
    Coach Station (measures and device specific data).
  termsOfService: https://dev.netatmo.com/dev/resources/legal/introduction
  contact:
    name: Netatmo
    email: contact-api@netatmo.com
  version: 1.1.1
host: api.netatmo.net
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devicelist:
    get:
      summary: Get Devicelist
      description: |-
        The method devicelist returns the list of devices owned by the user, and their modules.
        A device is identified by its _id (which is its mac address) and each device may have one, several or no modules, also identified by an _id.
      operationId: devicelist
      x-api-path-slug: devicelist-get
      parameters:
      - in: query
        name: app_type
        description: Defines which device type will be returned by devicelist
      - in: query
        name: device_id
        description: Specify a device_id if you want to retrieve only this device
          informations
      - in: query
        name: get_favorites
        description: When set to true, the favorite devices of the user are returned
      responses:
        200:
          description: OK
      tags:
      - Devices
  /gethomecoachsdata:
    get:
      summary: Get Gethomecoachsdata
      description: The method gethomecoachsdata Returns data from a user Healthy Home
        Coach Station (measures and device specific data).
      operationId: gethomecoachsdata
      x-api-path-slug: gethomecoachsdata-get
      parameters:
      - in: query
        name: device_id
        description: Id of the device you want to retrieve information of
      responses:
        200:
          description: OK
      tags:
      - Devices
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