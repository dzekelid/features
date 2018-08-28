{
  "info": {
    "name": "Dezrez Get feature suggestions for value",
    "_postman_id": "51e03173-109c-4d08-bb9c-965d83195874",
    "description": "Get feature suggestions for value.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "42b4939f-dbd8-409d-9a25-ceb081018052",
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
              "id": "140d8035-7415-4ecc-b616-5d0d7b9204af"
            }
          ]
        }
      ]
    },
    {
      "name": "Feature",
      "item": [
        {
          "id": "37dd7152-7b2d-4c06-92ee-89fd955614e7",
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
              "id": "8ddd71f6-a1a0-49f4-b26e-c0457e07f0b7"
            }
          ]
        },
        {
          "id": "1d1a4e24-b7cf-4e28-b881-bc8f7dc9549d",
          "name": "Feature_SuggestByname",
          "request": {
            "url": "http://api.dezrez.com/api/feature/suggest?name=%7B%7D",
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
            "description": "Get feature suggestions for value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8cae808-ef42-4401-9634-682c35528f83"
            }
          ]
        }
      ]
    }
  ]
}