{
  "info": {
    "name": "Dezrez Get a feature by its name",
    "_postman_id": "38672ed9-7297-4b1f-b97e-8e1073586ed0",
    "description": "Get a feature by its name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "d6a7dddd-e777-4c65-8ba8-849402fd570f",
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
              "id": "1bcadbef-346e-4627-88a1-60b093e24163"
            }
          ]
        }
      ]
    },
    {
      "name": "Feature",
      "item": [
        {
          "id": "b063929c-95ea-47c2-9712-6a3507034181",
          "name": "Feature_GetByname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/feature/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Get a feature by its name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1a4ee88-0814-44b5-8145-cb7a0a6fd763"
            }
          ]
        }
      ]
    }
  ]
}