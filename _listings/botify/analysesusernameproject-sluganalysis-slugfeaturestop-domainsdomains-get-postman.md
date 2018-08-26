{
  "info": {
    "name": "Botify Get Analyses Username Project Slug Analysis Slug Features Top Domains Domains",
    "_postman_id": "c6720a76-f638-4661-a2c1-6341c013808f",
    "description": "Get analyses username project slug analysis slug features top domains domains.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analyses",
      "item": [
        {
          "id": "ea2f9fc8-23b1-469f-925a-e89161938af0",
          "name": "getAnalysesUsernameProjectSlugAnalysisSlugFeaturesTopDomainsDomains",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.botify.com",
              "path": [
                "v1",
                "analyses/:username/:project_slug/:analysis_slug/features/top_domains/domains"
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
            "description": "Get analyses username project slug analysis slug features top domains domains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5072f676-f6f2-4578-8719-4ff59730b0b2"
            }
          ]
        }
      ]
    }
  ]
}