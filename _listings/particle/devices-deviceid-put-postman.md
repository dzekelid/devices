{
  "info": {
    "name": "Particle Put Devices Device",
    "_postman_id": "aff7a1a8-ed5f-43a3-80ec-ea773f8acd24",
    "description": "Flash a device.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "devices",
      "item": [
        {
          "id": "a56bae6d-5ae5-4cc8-bf33-83c4516e2db2",
          "name": "putDevicesDevice",
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
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "file",
                  "value": "{}",
                  "disabled": false,
                  "description": "The file to flash to the device"
                },
                {
                  "key": "file_type",
                  "value": "{}",
                  "disabled": false,
                  "description": "The type of the file being uploaded"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The desired name for the device"
                }
              ]
            },
            "description": "Flash a device"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae950ba0-3f4b-454c-b191-786278ffa1ba"
            }
          ]
        }
      ]
    }
  ]
}