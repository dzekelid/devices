---
swagger: "2.0"
x-collection-name: Netatmo
x-complete: 0
info:
  title: Netatmo Get Getthermostatsdata
  description: The method getthermostatsdata returns information about user's thermostats
    such as their last measurements.
  termsOfService: https://dev.netatmo.com/dev/resources/legal/introduction
  contact:
    name: Netatmo
    email: contact-api@netatmo.com
  version: 1.1.1
host: api.netatmo.net
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devicelist:
    get:
      summary: Get Devicelist
      description: |-
        The method devicelist returns the list of devices owned by the user, and their modules.
        A device is identified by its _id (which is its mac address) and each device may have one, several or no modules, also identified by an _id.
      operationId: devicelist
      x-api-path-slug: devicelist-get
      parameters:
      - in: query
        name: app_type
        description: Defines which device type will be returned by devicelist
      - in: query
        name: device_id
        description: Specify a device_id if you want to retrieve only this device
          informations
      - in: query
        name: get_favorites
        description: When set to true, the favorite devices of the user are returned
      responses:
        200:
          description: OK
      tags:
      - Devices
  /gethomecoachsdata:
    get:
      summary: Get Gethomecoachsdata
      description: The method gethomecoachsdata Returns data from a user Healthy Home
        Coach Station (measures and device specific data).
      operationId: gethomecoachsdata
      x-api-path-slug: gethomecoachsdata-get
      parameters:
      - in: query
        name: device_id
        description: Id of the device you want to retrieve information of
      responses:
        200:
          description: OK
      tags:
      - Devices
  /gethomedata:
    get:
      summary: Get Gethomedata
      description: Returns information about users homes and cameras.
      operationId: gethomedata
      x-api-path-slug: gethomedata-get
      parameters:
      - in: query
        name: home_id
        description: Specify if youre looking for the events of a specific Home
      - in: query
        name: size
        description: Number of events to retrieve
      responses:
        200:
          description: OK
      tags:
      - Devices
  /getlasteventof:
    get:
      summary: Get Getlasteventof
      description: Returns most recent events.
      operationId: getlasteventof
      x-api-path-slug: getlasteventof-get
      parameters:
      - in: query
        name: home_id
        description: ID of the Home youre interested in
      - in: query
        name: offset
        description: Number of events to retrieve
      - in: query
        name: person_id
        description: Your request will retrieve all events of the given home until
          the most recent event of the given person
      responses:
        200:
          description: OK
      tags:
      - Devices
  /getmeasure:
    get:
      summary: Get Getmeasure
      description: The method getmeasure returns the measurements of a device or a
        module.
      operationId: getmeasure
      x-api-path-slug: getmeasure-get
      parameters:
      - in: query
        name: date_begin
        description: Starting timestamp (utc) of the requested measurements
      - in: query
        name: date_end
        description: Ending timestamp (utc) of the request measurements
      - in: query
        name: device_id
        description: Id of the device whose modules measurements you want to retrieve
      - in: query
        name: limit
        description: Limits the number of measurements returned (default & max is
          1024)
      - in: query
        name: module_id
        description: If you dont specify any module_id you will retrieve the devices
          measurements
      - in: query
        name: optimize
        description: Allows you to choose the format of the answer
      - in: query
        name: real_time
        description: In scales higher than max, since the data is aggregated, the
          timestamps returned are by default offset by +(scale/2)
      - in: query
        name: scale
        description: Defines the time interval between two measurements
      - in: query
        name: type
        description: Sets the type of measurement you want to retrieve
      responses:
        200:
          description: OK
      tags:
      - Devices
  /getnextevents:
    get:
      summary: Get Getnextevents
      description: Returns previous events.
      operationId: getnextevents
      x-api-path-slug: getnextevents-get
      parameters:
      - in: query
        name: event_id
        description: Your request will retrieve events occured before this one
      - in: query
        name: home_id
        description: ID of the Home youre interested in
      - in: query
        name: size
        description: Number of events to retrieve
      responses:
        200:
          description: OK
      tags:
      - Devices
      - Events
  /getthermostatsdata:
    get:
      summary: Get Getthermostatsdata
      description: The method getthermostatsdata returns information about user's
        thermostats such as their last measurements.
      operationId: getthermostatsdata
      x-api-path-slug: getthermostatsdata-get
      parameters:
      - in: query
        name: device_id
        description: Id of the device you want to retrieve information of
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