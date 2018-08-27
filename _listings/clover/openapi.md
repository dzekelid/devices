---
swagger: "2.0"
x-collection-name: Clover
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/devices:
    get:
      summary: Get all devices provisioned to a merchant
      description: Returns a list of all devices that are provisioned to the a merchant.
        This list can be viewed from the Setup App on the merchant's device or web
        dashboard (https://www.clover.com/setupapp/m/{mId}/devices).
      operationId: GetMerchantDevices
      x-api-path-slug: v3merchantsmiddevices-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [id, model, name, orderPrefix, serial, deleted_time,
          merchant'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Devices
  /v3/merchants/{mId}/devices/{deviceId}:
    get:
      summary: Get a single device provisioned to a merchant
      description: Returns a single device that is provisioned to a merchant.
      operationId: GetMerchantDevice
      x-api-path-slug: v3merchantsmiddevicesdeviceid-get
      parameters:
      - in: path
        name: deviceId
        description: Device Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Devices
      - DeviceId
  /v3/merchants/{mId}/devices/{deviceId}/cash_events:
    get:
      summary: Get all cash events for a device
      description: Retrieve cash events filtered by device ID. Cash events can also
        be consumed by registering a Webhook callback. See https://docs.clover.com/build/webhooks/
      operationId: GetDeviceCashEvents
      x-api-path-slug: v3merchantsmiddevicesdeviceidcash-events-get
      parameters:
      - in: path
        name: deviceId
        description: Device Id
      - in: query
        name: expand
        description: 'Expandable fields: [employee, device]'
      - in: query
        name: filter
        description: 'Filter fields: [employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Devices
      - DeviceId
      - Cash
      - Events
  /v3/apps/{aId}/devices/{dId}/notifications:
    post:
      summary: Create a notification for a device
      description: 'Push a message to a device that has your app installed and is
        listening for notifications.  For details on how to use Clover''s Android
        SDK to receive notifications see: https://github.com/clover/android-examples/tree/master/pushnotificationexample'
      operationId: CreateDeviceAppNotification
      x-api-path-slug: v3appsaiddevicesdidnotifications-post
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: dId
        description: Developer Id
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Devices
      - DId
      - Notifications
---