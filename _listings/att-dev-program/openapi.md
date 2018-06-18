---
swagger: "2.0"
x-collection-name: AT&T Dev Program
x-complete: 1
info:
  title: AT&T API
  description: this-is-a-complete-definition-of-the-att-api--needs-to-be-broken-into-separate-endpoints-
  version: "1"
host: api.att.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/2/Devices/Info:
    get:
      summary: Get Devices Info
      description: /rest/2/Devices/Info
      operationId: rest2devicesinfo
      x-api-path-slug: rest2devicesinfo-get
      responses:
        200:
          description: OK
      tags:
      - Rest
      - Devices
      - Info
---