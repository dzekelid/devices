---
name: Actility
x-slug: actility
description: 'Actility is the leader in low power wide area (LoRaWAN and 3GPP) network
  connectivity management for the Internet of Things: the ThingPark platform'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
x-kinRank: "7"
x-alexaRank: "637591"
tags: Devices
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/apis.md
specificationVersion: "0.14"
apis:
- name: ThingPark DX Core API - Devices retrieval
  x-api-slug: devices-get
  description: 'Retrieves a list of devices existing within authorized scopes. Note
    that for each device, by default only the following information is retrieved:
    ''ref'', ''name'', ''EUI'', ''networkAddress''.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devices-get-openapi.md
- name: ThingPark DX Core API - Device creation
  x-api-slug: devices-post
  description: Creates a new device. If no 'routingProfileId' or 'processingStrategyId'
    values are provided, then 'processingStrategyId' will be automatically set to
    'DATAFLOW'. If no 'connectivityPlanId' value is provided, then the first connectivity
    plan of the subscriber with available connections will be assigned to the device.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devices-post-openapi.md
- name: ThingPark DX Core API - Device retrieval
  x-api-slug: devicesdeviceref-get
  description: Retrieves the device corresponding to the provided device ref, if that
    device is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicesdeviceref-get-openapi.md
- name: ThingPark DX Core API - Device update
  x-api-slug: devicesdeviceref-put
  description: 'Updates the device corresponding to the provided device ref, if that
    device is within authorized scopes. Only following attributes can be updated:
    ''name'', ''routingProfileId'', ''processingStrategyId'', ''connectivityPlanId'',
    ''deviceProfileId'' and ''applicationEUI''. To update other attributes, device
    must be deleted than re-created.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicesdeviceref-put-openapi.md
- name: ThingPark DX Core API - Device deletion
  x-api-slug: devicesdeviceref-delete
  description: Deletes the device corresponding to the provided device ref, if that
    device is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicesdeviceref-delete-openapi.md
- name: ThingPark DX Core API - Device profiles retrieval
  x-api-slug: deviceprofiles-get
  description: Retrieves the list of existing device profiles.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/deviceprofiles-get-openapi.md
- name: ThingPark DX Core API - Device alarms retrieval
  x-api-slug: devicealarms-get
  description: Retrieves a list of device alarms existing within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicealarms-get-openapi.md
- name: ThingPark DX Core API - Device alarm retrieval
  x-api-slug: devicealarmsdevicealarmref-get
  description: Retrieves the device alarm corresponding to the provided device alarm
    ref, if that device alarm is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicealarmsdevicealarmref-get-openapi.md
- name: ThingPark DX Core API - Device alarm acknowledgement
  x-api-slug: devicealarmsdevicealarmrefacks-post
  description: Acknowledges a device alarm.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicealarmsdevicealarmrefacks-post-openapi.md
- name: ThingPark DX Core API - Device alarm acknowledgement
  x-api-slug: devicealarmsdevicealarmrefacks-post
  description: Acknowledges a device alarm.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicealarmsdevicealarmrefacks-post-openapi.md
- name: ThingPark DX Core API - Device alarm retrieval
  x-api-slug: devicealarmsdevicealarmref-get
  description: Retrieves the device alarm corresponding to the provided device alarm
    ref, if that device alarm is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicealarmsdevicealarmref-get-openapi.md
- name: ThingPark DX Core API - Device alarms retrieval
  x-api-slug: devicealarms-get
  description: Retrieves a list of device alarms existing within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicealarms-get-openapi.md
- name: ThingPark DX Core API - Device profiles retrieval
  x-api-slug: deviceprofiles-get
  description: Retrieves the list of existing device profiles.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/deviceprofiles-get-openapi.md
- name: ThingPark DX Core API - Device deletion
  x-api-slug: devicesdeviceref-delete
  description: Deletes the device corresponding to the provided device ref, if that
    device is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicesdeviceref-delete-openapi.md
- name: ThingPark DX Core API - Device update
  x-api-slug: devicesdeviceref-put
  description: 'Updates the device corresponding to the provided device ref, if that
    device is within authorized scopes. Only following attributes can be updated:
    ''name'', ''routingProfileId'', ''processingStrategyId'', ''connectivityPlanId'',
    ''deviceProfileId'' and ''applicationEUI''. To update other attributes, device
    must be deleted than re-created.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicesdeviceref-put-openapi.md
- name: ThingPark DX Core API - Device retrieval
  x-api-slug: devicesdeviceref-get
  description: Retrieves the device corresponding to the provided device ref, if that
    device is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devicesdeviceref-get-openapi.md
- name: ThingPark DX Core API - Device creation
  x-api-slug: devices-post
  description: Creates a new device. If no 'routingProfileId' or 'processingStrategyId'
    values are provided, then 'processingStrategyId' will be automatically set to
    'DATAFLOW'. If no 'connectivityPlanId' value is provided, then the first connectivity
    plan of the subscriber with available connections will be assigned to the device.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/devices-post-openapi.md
- name: ThingPark DX Maker API - Factory devices retrieval
  x-api-slug: factorydevices-get
  description: Retrieves all factory devices.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//maker/v011/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/factorydevices-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/factorydevices-get-openapi.md
- name: ThingPark DX Maker API - Factory device creation
  x-api-slug: factorydevices-post
  description: Creates a factory device.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//maker/v011/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/factorydevices-post-openapi.md
- name: ThingPark DX Maker API - Factory device retrieval
  x-api-slug: factorydevicesfactorydeviceref-get
  description: Retrieves the factory device corresponding to the provided factoryDeviceRef.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//maker/v011/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/factorydevicesfactorydeviceref-get-openapi.md
- name: ThingPark DX Maker API - Factory device update
  x-api-slug: factorydevicesfactorydeviceref-put
  description: Updates the factory device corresponding to the provided factoryDeviceRef.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//maker/v011/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/factorydevicesfactorydeviceref-put-openapi.md
- name: ThingPark DX Maker API - Factory device deletion
  x-api-slug: factorydevicesfactorydeviceref-delete
  description: Deletes the factory device corresponding to the provided factoryDeviceRef.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//maker/v011/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/factorydevicesfactorydeviceref-delete-openapi.md
- name: ThingPark DX Maker API - Factory device deletion
  x-api-slug: factorydevicesfactorydeviceref-delete
  description: Deletes the factory device corresponding to the provided factoryDeviceRef.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//maker/v011/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/factorydevicesfactorydeviceref-delete-openapi.md
- name: ThingPark DX Maker API - Factory device update
  x-api-slug: factorydevicesfactorydeviceref-put
  description: Updates the factory device corresponding to the provided factoryDeviceRef.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//maker/v011/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/factorydevicesfactorydeviceref-put-openapi.md
- name: ThingPark DX Maker API - Factory device retrieval
  x-api-slug: factorydevicesfactorydeviceref-get
  description: Retrieves the factory device corresponding to the provided factoryDeviceRef.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//maker/v011/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/factorydevicesfactorydeviceref-get-openapi.md
- name: ThingPark DX Maker API - Factory device creation
  x-api-slug: factorydevices-post
  description: Creates a factory device.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//maker/v011/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/devices/master/_listings/actility/factorydevices-post-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.actility.com/blog/feed/
- type: x-github
  url: https://github.com/actility
- type: x-openapi
  url: https://dx-api.thingpark.com/core/latest/tpdx-core-api-contract.json
- type: x-api-gallery
  url: http://actility.api.gallery.streamdata.io
- type: x-api-stack
  url: http://actility.stack.network
- type: x-blog
  url: https://www.actility.com/blog/
- type: x-crunchbase
  url: https://crunchbase.com/organization/actility
- type: x-developer
  url: https://www.actility.com/developer/
- type: x-twitter
  url: https://twitter.com/Actility
- type: x-website
  url: https://www.actility.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---