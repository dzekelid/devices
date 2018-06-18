---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API List Devices
  version: 1.0.0
  description: Lists the devices.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AdminForgetDevice:
    get:
      summary: Admin Forget Device
      description: Forgets the device, as an administrator.
      operationId: adminForgetDevice
      x-api-path-slug: actionadminforgetdevice-get
      parameters:
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=ConfirmDevice:
    get:
      summary: Confirm Device
      description: Confirms tracking of the device.
      operationId: confirmDevice
      x-api-path-slug: actionconfirmdevice-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token
        type: string
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: DeviceName
        description: The device name
        type: string
      - in: query
        name: DeviceSecretVerifierConfig
        description: The configuration of the device secret verifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=ForgetDevice:
    get:
      summary: Forget Device
      description: Forgets the specified device.
      operationId: forgetDevice
      x-api-path-slug: actionforgetdevice-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token for the forgotten device request
        type: string
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=ListDevices:
    get:
      summary: List Devices
      description: Lists the devices.
      operationId: listDevices
      x-api-path-slug: actionlistdevices-get
      parameters:
      - in: query
        name: AccessToken
        description: The access tokens for the request to list devices
        type: string
      - in: query
        name: Limit
        description: The limit of the device request
        type: string
      - in: query
        name: PaginationToken
        description: The pagination token for the list request
        type: string
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