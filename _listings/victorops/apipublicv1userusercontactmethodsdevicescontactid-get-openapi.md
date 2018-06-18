---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 0
info:
  title: Victor Ops Get the indicated contact device for a user
  description: |-
    Get the indicated contact device for a user

    This API may be called a maximum of 15 times per minute.
  version: 0.0.2
host: api.victorops.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-public/v1/user/{user}/contact-methods/devices:
    get:
      summary: Get a list of all contact devices for a user
      description: |-
        Get the contact methods for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.devices.get
      x-api-path-slug: apipublicv1userusercontactmethodsdevices-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Contact-methods
      - Devices
  /api-public/v1/user/{user}/contact-methods/devices/{contactId}:
    delete:
      summary: Delete a contact device for a user
      description: |-
        Delete a contact device for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.devices.contactId.delete
      x-api-path-slug: apipublicv1userusercontactmethodsdevicescontactid-delete
      parameters:
      - in: path
        name: contactId
        description: The unique contact identifier
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Contact-methods
      - Devices
      - ContactId
    get:
      summary: Get the indicated contact device for a user
      description: |-
        Get the indicated contact device for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.devices.contactId.get
      x-api-path-slug: apipublicv1userusercontactmethodsdevicescontactid-get
      parameters:
      - in: path
        name: contactId
        description: The unique contact identifier
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Contact-methods
      - Devices
      - ContactId
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