---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox for Business API
  description: the-business-version-of-the-dropbox-api-
  version: "1"
host: api.dropbox.com
basePath: /1/team
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/get_devices:
    post:
      summary: Get Devices
      description: Get devices.
      operationId: postReportsGetDevices
      x-api-path-slug: reportsget-devices-post
      parameters:
      - in: query
        name: end_date
        description: optional ending date (exclusive)
      - in: query
        name: start_date
        description: optional starting date (inclusive)
      responses:
        200:
          description: OK
      tags:
      - Devices
---