{
  "info": {
    "name": "Particle Add Devices",
    "_postman_id": "80cd5159-bf00-4c5e-a3a9-7119a1eb2060",
    "description": "Claim a new or unclaimed device to your account or request transfer from another user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "devices",
      "item": [
        {
          "id": "f67390da-4ab7-42d7-bb3c-41778fbc0285",
          "name": "postDevices",
          "request": {
            "url": "http://api.particle.io/v1/devices?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "request_transfer",
                  "value": "{}",
                  "disabled": false,
                  "description": "Include this and set to true to request transfer of an existing device"
                }
              ]
            },
            "description": "Claim a new or unclaimed device to your account or request transfer from another user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b18fdb20-b36a-4ab2-8d48-a502773079be"
            }
          ]
        }
      ]
    }
  ]
}