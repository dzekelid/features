{
  "info": {
    "name": "Botify Get Analyses Username Project Slug Analysis Slug Features Top Domains Subdomains",
    "_postman_id": "32ddfa7d-5cc0-406a-a325-03b649b16a40",
    "description": "Get analyses username project slug analysis slug features top domains subdomains.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analyses",
      "item": [
        {
          "id": "4840ba14-795b-4710-8fff-1b1548c06096",
          "name": "getAnalysesUsernameProjectSlugAnalysisSlugFeaturesTopDomainsSubdomains",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.botify.com",
              "path": [
                "v1",
                "analyses/:username/:project_slug/:analysis_slug/features/top_domains/subdomains"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "size",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Get analyses username project slug analysis slug features top domains subdomains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c7dd0cb-dfb9-4835-b826-c1524beac866"
            }
          ]
        }
      ]
    }
  ]
}