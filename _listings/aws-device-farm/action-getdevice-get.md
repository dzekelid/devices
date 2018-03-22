---
swagger: "2.0"
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
      summary: ' Get Device '
      description: Gets information about a unique device type
      operationId: getDevice
      parameters:
      - in: query
        name: arn
        description: The device type's ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - devices
definitions: []
x-collection-name: AWS Device Farm
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