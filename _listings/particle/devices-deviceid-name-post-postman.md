{
  "info": {
    "name": "Particle Add Devices Device Name",
    "_postman_id": "6bf42ea4-56e6-452f-b026-aa5c22abdc98",
    "description": "Call a function exposed by the device, with arguments passed in the request body.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "devices",
      "item": [
        {
          "id": "e299b7e6-2590-4046-924d-c5f07be180d1",
          "name": "postDevicesDeviceName",
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
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "arg",
                  "value": "{}",
                  "disabled": false,
                  "description": "Function argument"
                }
              ]
            },
            "description": "Call a function exposed by the device, with arguments passed in the request body"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ac734b4-76c2-480b-bbe1-555813290ca3"
            }
          ]
        }
      ]
    }
  ]
}