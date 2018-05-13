{
  "info": {
    "name": "Particle Get Devices Device Name",
    "_postman_id": "ae084b6a-05aa-431d-918c-d5be161a5588",
    "description": "Request the current value of a variable exposed by the device.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "devices",
      "item": [
        {
          "id": "ac2a4571-93a6-4a2f-8763-f54f0a8a73ff",
          "name": "getDevicesDeviceName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.particle.io",
              "path": [
                "v1",
                "devices/:deviceID/:name"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "deviceID",
                  "value": "deviceID",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request the current value of a variable exposed by the device"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c7f886f-872e-4601-87ac-122a821fd6ee"
            }
          ]
        }
      ]
    }
  ]
}