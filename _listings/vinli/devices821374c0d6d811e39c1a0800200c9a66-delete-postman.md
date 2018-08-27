{
  "info": {
    "name": "Vinli Deregister a Device",
    "_postman_id": "d8b790e5-6da7-4b2f-bc64-417c36d9d276",
    "description": "Deregister a device.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Deregister",
      "item": [
        {
          "id": "622201f3-7779-46b9-b809-3ecf87cef83c",
          "name": "Devices821374c0D6d811e39c1a0800200c9a66Delete",
          "request": {
            "url": "http://events.vin.li/api/v1/devices/821374c0-d6d8-11e3-9c1a-0800200c9a66",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deregister a device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f5b56dd-318a-4d15-a2f7-d654408de6f4"
            }
          ]
        }
      ]
    }
  ]
}