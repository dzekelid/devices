{
  "info": {
    "name": "Vinli get a single device",
    "_postman_id": "c74d2ca2-d876-434a-9f13-78aee627bd89",
    "description": "Get a single device.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "7915e4d8-7d13-4f28-96d5-860c5b6ebbd2",
          "name": "DevicesCf217c2dDf3c41f7B6108bc3e11b4b79Get",
          "request": {
            "url": "http://events.vin.li/api/v1/devices/cf217c2d-df3c-41f7-b610-8bc3e11b4b79",
            "method": "GET",
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
            "description": "Get a single device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac28577c-ac4d-4801-b704-4dfd5d7ffbb9"
            }
          ]
        }
      ]
    }
  ]
}