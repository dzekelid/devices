---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: NxtPort Big Belly API Publish Device
  description: Publish the fill level for all Big Belly devices.
  termsOfService: https://www.nxtport.eu/General-Terms-And-Conditions
  version: 1.0.0
host: api-stg.nxtport.eu
basePath: /bigbelly/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices:
    post:
      summary: Publish Device
      description: Publish the fill level for all Big Belly devices.
      operationId: Publish_Devices
      x-api-path-slug: devices-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
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