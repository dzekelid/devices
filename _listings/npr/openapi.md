swagger: "2.0"
x-collection-name: NPR
x-complete: 1
info:
  title: NPR One API Reference
  description: npr-one-is-a-smart-application-that-brings-the-best-of-npr-and-member-station-programming-newscasts-podcasts-and-stories-together-to-create-a-new-experience-for-listening--it-provides-an-editorcurated-and-localized-mobile-listening-experience-based-on-the-content-the-listener-chooses-likes-shares-and-enjoys--the-api-provides-all-of-the-content-and-customization-in-a-simple-structured-way-that-is-easy-for-applicationdevelopers-to-implement-
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