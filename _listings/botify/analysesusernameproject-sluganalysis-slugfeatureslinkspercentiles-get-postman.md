{
  "info": {
    "name": "Botify Get Analyses Username Project Slug Analysis Slug Features Links Percentiles",
    "_postman_id": "f5a9ca71-f92e-4bd3-95eb-14fd002963bd",
    "description": "Get analyses username project slug analysis slug features links percentiles.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analyses",
      "item": [
        {
          "id": "4acc13ac-1edc-4831-bcbf-1ea7b4a73233",
          "name": "getAnalysesUsernameProjectSlugAnalysisSlugFeaturesLinksPercentiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.botify.com",
              "path": [
                "v1",
                "analyses/:username/:project_slug/:analysis_slug/features/links/percentiles"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "project_slug",
                  "value": "project_slug",
                  "type": "string"
                },
                {
                  "id": "analysis_slug",
                  "value": "analysis_slug",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get analyses username project slug analysis slug features links percentiles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2126255f-d9d7-4017-9bb5-9c7734d69185"
            }
          ]
        }
      ]
    }
  ]
}