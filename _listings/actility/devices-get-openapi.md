---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Core API Devices retrieval
  description: 'Retrieves a list of devices existing within authorized scopes. Note
    that for each device, by default only the following information is retrieved:
    ''ref'', ''name'', ''EUI'', ''networkAddress''.'
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /core/v141/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices:
    get:
      summary: Devices retrieval
      description: 'Retrieves a list of devices existing within authorized scopes.
        Note that for each device, by default only the following information is retrieved:
        ''ref'', ''name'', ''EUI'', ''networkAddress''.'
      operationId: retrieves-a-list-of-devices-existing-within-authorized-scopes-note-that-for-each-device-by-default-o
      x-api-path-slug: devices-get
      parameters:
      - in: query
        name: commercialDetails
        description: Indicates to also retrieve commercial information along each
          device
      - in: query
        name: connectivityPlanId
        description: Connectivity plan assigned to the devices to search for
      - in: query
        name: deviceEUI
        description: EUI of the device to search for
      - in: query
        name: deviceToken
        description: Token provided by the manufacturer for an easy registration on
          a standalone Join Server
      - in: query
        name: extendedInfo
        description: Indicates to retrieve all available information (including statistics
          and commercial details) along each device
      - in: query
        name: healthState
        description: Health state of the devices to search for
      - in: query
        name: pageIndex
        description: If set, enables pagination and returns only the 100 devices of
          the specified page
      - in: query
        name: statistics
        description: Indicates to also retrieve usage statistic information along
          each device
      responses:
        200:
          description: OK
      tags:
      - Devices
      - Retrieval
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