---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 1
info:
  title: Victor Ops
  description: this-api-allows-you-to-interact-with-the-victorops-platform-in-various-ways--your-account-may-be-limitedto-a-total-number-of-api-calls-per-month--also-some-of-these-api-calls-have-rate-limits-note-in-this-documentation-when-creating-a-sample-curl-request-clicking-the-try-it-out-button-in-some-apiviewing-interfaces-the--in-an-email-address-may-be-encoded--please-note-that-the-rest-endpoints-will-notprocess-the-encoded-version--make-sure-that-the-encoded-character-40-is-changed-to-its-unencoded-form-beforesubmitting-the-curl-request-
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
    put:
      summary: Update a contact device for a user
      description: |-
        Update a contact device for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.devices.contactId.put
      x-api-path-slug: apipublicv1userusercontactmethodsdevicescontactid-put
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
---