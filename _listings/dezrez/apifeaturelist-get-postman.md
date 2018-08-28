{
  "info": {
    "name": "Dezrez Get  a list of features by a list of ids",
    "_postman_id": "fddbbb74-12c1-4c61-98ee-fab66602168e",
    "description": "Get  a list of features by a list of ids.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "8df6a7b1-3c6d-4285-8165-05a4f02a8c93",
          "name": "Feature_GetByfeatureid",
          "request": {
            "url": "http://api.dezrez.com/api/feature/list?featureid=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get  a list of features by a list of ids."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "841fdc62-9610-4095-80db-c8685101d9af"
            }
          ]
        }
      ]
    }
  ]
}