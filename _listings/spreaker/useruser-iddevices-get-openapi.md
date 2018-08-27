---
swagger: "2.0"
x-collection-name: Spreaker
x-complete: 0
info:
  title: Spreaker API Create Device
  version: v1
  description: Creates a new device.
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/{user_id}/device/{token}:
    delete:
      summary: Delete Device
      description: Delete the association from a mobile device and a registered user
      operationId: deleteUserUserDeviceToken
      x-api-path-slug: useruser-iddevicetoken-delete
      parameters:
      - in: path
        name: token
        description: The device token
      - in: path
        name: user_id
        description: The user id
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
        200:
          description: OK
      tags:
      - Podcasts
      - Device
  /user/{user_id}/devices:
    get:
      summary: Create Device
      description: Creates a new device.
      operationId: getUserUserDevices
      x-api-path-slug: useruser-iddevices-get
      parameters:
      - in: query
        name: application_id
        description: The application related to the request
      - in: path
        name: Delete Device
        description: The user id
      - in: query
        name: device_name
        description: The device name, max length 255
      - in: query
        name: device_token
        description: The device token, max length 255
      responses:
        200:
          description: OK
      tags:
      - Podcasts
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