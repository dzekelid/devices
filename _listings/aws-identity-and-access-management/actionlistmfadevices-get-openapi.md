---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API List M F A Devices
  version: 1.0.0
  description: Lists the MFA devices for an IAM user.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListMFADevices:
    get:
      summary: List M F A Devices
      description: Lists the MFA devices for an IAM user.
      operationId: listMFADevices
      x-api-path-slug: actionlistmfadevices-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the user whose MFA devices you want to list
        type: string
      responses:
        200:
          description: OK
      tags:
      - MFA Devices
  /?Action=ListVirtualMFADevices:
    get:
      summary: List Virtual M F A Devices
      description: Lists the virtual MFA devices defined in the AWS account by assignment
        status.
      operationId: listVirtualMFADevices
      x-api-path-slug: actionlistvirtualmfadevices-get
      parameters:
      - in: query
        name: AssignmentStatus
        description: The status (Unassigned or Assigned) of the devices to list
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Virtual MFA Devices
  /?Action=CreateVirtualMFADevice:
    get:
      summary: Create Virtual M F A Device
      description: Creates a new virtual MFA device for the AWS account.
      operationId: createVirtualMFADevice
      x-api-path-slug: actioncreatevirtualmfadevice-get
      parameters:
      - in: query
        name: Path
        description: The path for the virtual MFA device
        type: string
      - in: query
        name: VirtualMFADeviceName
        description: The name of the virtual MFA device
        type: string
      responses:
        200:
          description: OK
      tags:
      - Virtual MFA Device
  /?Action=DeactivateMFADevice:
    get:
      summary: Deactivate M F A Device
      description: |-
        Deactivates the specified MFA device and removes it from association with the user name
              for which it was originally enabled.
      operationId: deactivateMFADevice
      x-api-path-slug: actiondeactivatemfadevice-get
      parameters:
      - in: query
        name: SerialNumber
        description: The serial number that uniquely identifies the MFA device
        type: string
      - in: query
        name: UserName
        description: The name of the user whose MFA device you want to deactivate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Virtual MFA Device
  /?Action=DeleteVirtualMFADevice:
    get:
      summary: Delete Virtual M F A Device
      description: Deletes a virtual MFA device.
      operationId: deleteVirtualMFADevice
      x-api-path-slug: actiondeletevirtualmfadevice-get
      parameters:
      - in: query
        name: SerialNumber
        description: The serial number that uniquely identifies the MFA device
        type: string
      responses:
        200:
          description: OK
      tags:
      - Virtual MFA Devices
  /?Action=EnableMFADevice:
    get:
      summary: Enable M F A Device
      description: Enables the specified MFA device and associates it with the specified
        IAM user.
      operationId: enableMFADevice
      x-api-path-slug: actionenablemfadevice-get
      parameters:
      - in: query
        name: AuthenticationCode1
        description: An authentication code emitted by the device
        type: string
      - in: query
        name: AuthenticationCode2
        description: A subsequent authentication code emitted by the device
        type: string
      - in: query
        name: SerialNumber
        description: The serial number that uniquely identifies the MFA device
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user for whom you want to enable the MFA
          device
        type: string
      responses:
        200:
          description: OK
      tags:
      - MFA Devices
  /?Action=ResyncMFADevice:
    get:
      summary: Resync M F A Device
      description: |-
        Synchronizes the specified MFA device with its IAM resource object on the AWS
              servers.
      operationId: resyncMFADevice
      x-api-path-slug: actionresyncmfadevice-get
      parameters:
      - in: query
        name: AuthenticationCode1
        description: An authentication code emitted by the device
        type: string
      - in: query
        name: AuthenticationCode2
        description: A subsequent authentication code emitted by the device
        type: string
      - in: query
        name: SerialNumber
        description: Serial number that uniquely identifies the MFA device
        type: string
      - in: query
        name: UserName
        description: The name of the user whose MFA device you want to resynchronize
        type: string
      responses:
        200:
          description: OK
      tags:
      - MFA Devices
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