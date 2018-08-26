{
  "info": {
    "name": "Data.gov API Add Datasets Dataset Featured",
    "_postman_id": "e97a0d34-980b-4857-a3b1-659582866d61",
    "description": "Mark the dataset as featured",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "a47359d4-177d-41f0-ad57-4c8b4ced5805",
          "name": "postDatasetsDatasetFeatured",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "datasets/:dataset/featured/"
              ],
              "variable": [
                {
                  "id": "dataset",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Mark the dataset as featured"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2b569dc-0564-4c33-b809-c8710715bdd3"
            }
          ]
        }
      ]
    }
  ]
}