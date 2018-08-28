---
swagger: "2.0"
x-collection-name: NPR
x-complete: 0
info:
  title: NPR Initiate an OAuth2 login flow for limited input devices
  description: |-
    This flow should only be used by clients who cannot show a native webview or do not have advanced input controls. It is an alternative to `GET /authorization/v2/authorize`.

    Third-party clients will need to use one or the other of these two endpoints, but they will generally not use both.
  termsOfService: http://dev.npr.org/develop/terms-of-use
  contact:
    name: NPR One Enterprise Team
    url: http://dev.npr.org
    email: NPROneEnterprise@npr.org
  version: 1.0.0
host: api.npr.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /authorization/v2/device:
    post:
      summary: Initiate an OAuth2 login flow for limited input devices
      description: |-
        This flow should only be used by clients who cannot show a native webview or do not have advanced input controls. It is an alternative to `GET /authorization/v2/authorize`.

        Third-party clients will need to use one or the other of these two endpoints, but they will generally not use both.
      operationId: generateDeviceCode
      x-api-path-slug: authorizationv2device-post
      parameters:
      - in: formData
        name: client_id
        description: The clients ID
      - in: formData
        name: client_secret
        description: The clients secret key
      - in: formData
        name: scope
        description: A space-separated list of scope(s) requested by the application
      responses:
        200:
          description: OK
      tags:
      - News
      - Authorization
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