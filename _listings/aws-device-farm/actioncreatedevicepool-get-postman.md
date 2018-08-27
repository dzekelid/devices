{
  "info": {
    "name": "AWS Device Farm API Create Device Pool",
    "_postman_id": "34fd807f-2dcd-4a4b-a306-dfc9a6f68c0c",
    "description": "Creates a device pool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device Pool",
      "item": [
        {
          "id": "cf39a704-a0cb-4e53-b8a7-475b5885c868",
          "name": "createDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=CreateDevicePool?description=description&name=name&projectArn=projectArn&rules=rules",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "824d7faa-a716-4be6-80fe-365a6d61690e"
            }
          ]
        }
      ]
    }
  ]
}