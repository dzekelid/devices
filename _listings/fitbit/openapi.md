---
swagger: "2.0"
x-collection-name: Fitbit
x-complete: 1
info:
  title: Fitbit
  description: bring-fitbit-health-data-into-your-apps-including-user-activities-sleep-heart-glucose-and-blood-pressure-information-
  version: 1.0.0
host: api.fitbit.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/-/devices.json:
    get:
      summary: Get User Devices.json
      description: Retrieve the list of Fitbit devices for a user in the format requested.
      operationId: getUserDevices.json
      x-api-path-slug: userdevices-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Devices.json
---