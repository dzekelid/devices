{
  "info": {
    "name": "Particle Get Devices",
    "_postman_id": "e3d0e4a7-2e03-45d5-9eed-4fdb0bdf0cf3",
    "description": "List devices the currently authenticated user has access to.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "devices",
      "item": [
        {
          "id": "471c596b-a20f-4114-932e-ad384e957fda",
          "name": "getDevices",
          "request": {
            "url": "http://api.particle.io/v1/devices",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List devices the currently authenticated user has access to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af432a69-e527-48ca-bd56-49b99b6a4362"
            }
          ]
        }
      ]
    }
  ]
}