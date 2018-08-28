---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Edit Paging Group Users and Devices
  description: "Adds and/or removes paging group users and devices.\nApp Permission\nEditAccounts\nUser
    Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [addedDeviceIds]
    value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [EditAccounts] permission"
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/account/{accountId}/paging-only-groups/{pagingOnlyGroupId}/devices:
    get:
      summary: Get Paging Only Group Devices
      description: "Returns the list of paging devices assigned to this group.\nApp
        Permission\nReadAccounts\nUser Permission\nReadCompanyDevices\nUsage Plan
        Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application
        needs to have [ReadAccounts] permission"
      operationId: listPagingGroupDevices
      x-api-path-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get
      parameters:
      - in: path
        name: accountId
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: path
        name: pagingOnlyGroupId
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Paging
      - Only
      - Group
      - Devices
  /restapi/v1.0/account/{accountId}/paging-only-groups/{pagingOnlyGroupId}/bulk-assign:
    post:
      summary: Edit Paging Group Users and Devices
      description: "Adds and/or removes paging group users and devices.\nApp Permission\nEditAccounts\nUser
        Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n
        \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [addedDeviceIds] value is invalid\n\n\n403\nCMN-401\nIn order to call this
        API endpoint, application needs to have [EditAccounts] permission"
      operationId: bulkAssignPagingGroup
      x-api-path-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post
      parameters:
      - in: path
        name: accountId
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: pagingOnlyGroupId
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Paging
      - Group
      - Users
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