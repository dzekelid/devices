---
swagger: "2.0"
x-collection-name: Vinli
x-complete: 0
info:
  title: Vinli Create a Dummy Device
  description: Create a dummy device.
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices/cf217c2d-df3c-41f7-b610-8bc3e11b4b79/vehicles:
    get:
      summary: List a Device's Vehicles
      description: List a device's vehicles.
      operationId: DevicesCf217c2dDf3c41f7B6108bc3e11b4b79VehiclesGet
      x-api-path-slug: devicescf217c2ddf3c41f7b6108bc3e11b4b79vehicles-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - Devices
      - Vehicles
  /devices:
    get:
      summary: List all devices
      description: List all devices.
      operationId: DevicesGet
      x-api-path-slug: devices-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Devices
    post:
      summary: Register a Device
      description: Register a device.
      operationId: DevicesPost
      x-api-path-slug: devices-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Register
      - Device
  /devices/821374c0-d6d8-11e3-9c1a-0800200c9a66/vehicles/_latest:
    get:
      summary: Get Device's Latest Vehicle
      description: Get device's latest vehicle.
      operationId: Devices821374c0D6d811e39c1a0800200c9a66VehiclesLatestGet
      x-api-path-slug: devices821374c0d6d811e39c1a0800200c9a66vehicles-latest-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Devices
      - Latest
      - Vehicle
  /dummies:
    get:
      summary: List Dummy Devices
      description: List dummy devices.
      operationId: DummiesGet
      x-api-path-slug: dummies-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - Dummy
      - Devices
    post:
      summary: Create a Dummy Device
      description: Create a dummy device.
      operationId: DummiesPost
      x-api-path-slug: dummies-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Dummy
      - Device
  /devices/cf217c2d-df3c-41f7-b610-8bc3e11b4b79/trips:
    get:
      summary: List All of a Device's Trips
      description: List all of a device's trips.
      operationId: DevicesCf217c2dDf3c41f7B6108bc3e11b4b79TripsGet
      x-api-path-slug: devicescf217c2ddf3c41f7b6108bc3e11b4b79trips-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Of
      - Devices
      - Trips
  /devices/62976d30-b6dc-40f1-8422-ccc367572101/events:
    get:
      summary: Get All Events for a Device
      description: Get all events for a device.
      operationId: Devices62976d30B6dc40f18422Ccc367572101EventsGet
      x-api-path-slug: devices62976d30b6dc40f18422ccc367572101events-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Eventsa
      - Device
  /devices/7eac0d62-854f-41c1-a5b2-ba13c460058a/collisions:
    get:
      summary: Get a List of Collisions for a Device
      description: Get a list of collisions for a device.
      operationId: Devices7eac0d62854f41c1A5b2Ba13c460058aCollisionsGet
      x-api-path-slug: devices7eac0d62854f41c1a5b2ba13c460058acollisions-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Collisionsa
      - Device
  /devices/62976d30-b6dc-40f1-8422-ccc367572101/subscriptions:
    get:
      summary: Get all Subscriptions for a Device
      description: Get all subscriptions for a device.
      operationId: Devices62976d30B6dc40f18422Ccc367572101SubscriptionsGet
      x-api-path-slug: devices62976d30b6dc40f18422ccc367572101subscriptions-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Subscriptionsa
      - Device
  /devices/cf217c2d-df3c-41f7-b610-8bc3e11b4b79:
    get:
      summary: get a single device
      description: Get a single device.
      operationId: DevicesCf217c2dDf3c41f7B6108bc3e11b4b79Get
      x-api-path-slug: devicescf217c2ddf3c41f7b6108bc3e11b4b79-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Single
      - Device
  /devices/7eac0d62-854f-41c1-a5b2-ba13c460058a/report_cards/overall:
    get:
      summary: Lifetime Report Card for a Device
      description: Lifetime report card for a device.
      operationId: Devices7eac0d62854f41c1A5b2Ba13c460058aReportCardsOverallGet
      x-api-path-slug: devices7eac0d62854f41c1a5b2ba13c460058areport-cardsoverall-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Lifetime
      - Report
      - Carda
      - Device
  /devices/62976d30-b6dc-40f1-8422-ccc367572101/rules:
    post:
      summary: Create a Rule for a Device
      description: Create a rule for a device.
      operationId: Devices62976d30B6dc40f18422Ccc367572101RulesPost
      x-api-path-slug: devices62976d30b6dc40f18422ccc367572101rules-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Rulea
      - Device
  /devices/7eac0d62-854f-41c1-a5b2-ba13c460058a/report_cards:
    get:
      summary: Report Cards for a Device
      description: Report cards for a device.
      operationId: Devices7eac0d62854f41c1A5b2Ba13c460058aReportCardsGet
      x-api-path-slug: devices7eac0d62854f41c1a5b2ba13c460058areport-cards-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Report
      - Cardsa
      - Device
  /devices/cf217c2d-df3c-41f7-b610-8bc3e11b4b79/rules:
    get:
      summary: List all Rules for a Device
      description: List all rules for a device.
      operationId: DevicesCf217c2dDf3c41f7B6108bc3e11b4b79RulesGet
      x-api-path-slug: devicescf217c2ddf3c41f7b6108bc3e11b4b79rules-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Rulesa
      - Device
  /devices/821374c0-d6d8-11e3-9c1a-0800200c9a66:
    delete:
      summary: Deregister a Device
      description: Deregister a device.
      operationId: Devices821374c0D6d811e39c1a0800200c9a66Delete
      x-api-path-slug: devices821374c0d6d811e39c1a0800200c9a66-delete
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Device
  /vehicles/9aa35c64-b046-43cc-9cd8-4c353a6d0b30/codes:
    get:
      summary: List all DTCs for a Device
      description: List all dtcs for a device.
      operationId: Vehicles9aa35c64B04643cc9cd84c353a6d0b30CodesGet
      x-api-path-slug: vehicles9aa35c64b04643cc9cd84c353a6d0b30codes-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - DTCsa
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