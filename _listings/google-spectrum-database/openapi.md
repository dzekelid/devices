---
swagger: "2.0"
x-collection-name: Google Spectrum Database
x-complete: 1
info:
  title: Google Spectrum Database
  description: api-for-spectrummanagement-functions-
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
---