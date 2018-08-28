---
swagger: "2.0"
x-collection-name: Google Spectrum Database
x-complete: 0
info:
  title: Google Spectrum Database API Verify Device
  description: Validates a device for white space use in accordance with regulatory
    rules. The Google Spectrum Database does not support master/slave configurations,
    so this always yields an UNIMPLEMENTED error.
  contact:
    name: Google
    url: https://google.com
  version: v1explorer
host: www.googleapis.com
basePath: /spectrum/v1explorer/paws
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /verifyDevice:
    post:
      summary: Verify Device
      description: Validates a device for white space use in accordance with regulatory
        rules. The Google Spectrum Database does not support master/slave configurations,
        so this always yields an UNIMPLEMENTED error.
      operationId: spectrum.paws.verifyDevice
      x-api-path-slug: verifydevice-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
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