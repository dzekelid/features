{
  "info": {
    "name": "Botify Get Analyses Username Project Slug Analysis Slug Features Sitemaps Report",
    "_postman_id": "26d0f531-fcdd-4c95-9df1-cd08e8229a54",
    "description": "Get global information of the sitemaps found (sitemaps indexes, invalid sitemaps urls, etc.)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analyses",
      "item": [
        {
          "id": "e34b047a-be1a-46cf-92f5-370f88f31d37",
          "name": "getAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsReport",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.botify.com",
              "path": [
                "v1",
                "analyses/:username/:project_slug/:analysis_slug/features/sitemaps/report"
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
            "description": "Get global information of the sitemaps found (sitemaps indexes, invalid sitemaps urls, etc.)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f1e7213-9c4d-473c-b3aa-4a3384f4a954"
            }
          ]
        }
      ]
    }
  ]
}