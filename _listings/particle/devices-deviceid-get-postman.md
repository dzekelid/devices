{
  "info": {
    "name": "Particle Get Devices Device",
    "_postman_id": "0c8b13e8-5924-4677-a360-c7a89b4b69d1",
    "description": "Get basic information about the given device, including the custom variables and functions it has exposed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "devices",
      "item": [
        {
          "id": "151014cb-ba65-49a1-bc1e-7ff22a8d4d4b",
          "name": "getDevicesDevice",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.particle.io",
              "path": [
                "v1",
                "devices/:deviceID"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
            "description": "Get basic information about the given device, including the custom variables and functions it has exposed"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "562b5e64-59e7-464f-82ea-7761c48ff5f0"
            }
          ]
        }
      ]
    }
  ]
}