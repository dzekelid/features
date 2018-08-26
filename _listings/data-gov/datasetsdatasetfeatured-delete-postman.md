{
  "info": {
    "name": "Data.gov API Delete Datasets Dataset Featured",
    "_postman_id": "da26aa86-817c-4c63-aff3-92b175c97285",
    "description": "Unmark the dataset as featured",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "760adbd7-da07-40bd-be3b-16bf42645688",
          "name": "deleteDatasetsDatasetFeatured",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unmark the dataset as featured"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "382d2ff9-8bb3-44c8-9670-3858ad9f7303"
            }
          ]
        }
      ]
    }
  ]
}