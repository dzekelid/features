{
  "info": {
    "name": "Botify Get Analyses Username Project Slug Analysis Slug Features Pagerank Lost",
    "_postman_id": "7665e918-f6be-42f1-9c1f-22548262bc5c",
    "description": "Get analyses username project slug analysis slug features pagerank lost.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analyses",
      "item": [
        {
          "id": "d7a51408-d5e8-4bc5-a902-f97238eae05e",
          "name": "getAnalysesUsernameProjectSlugAnalysisSlugFeaturesPagerankLost",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.botify.com",
              "path": [
                "v1",
                "analyses/:username/:project_slug/:analysis_slug/features/pagerank/lost"
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
            "description": "Get analyses username project slug analysis slug features pagerank lost."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2bd4429-1365-4a61-9781-f300fc28029e"
            }
          ]
        }
      ]
    }
  ]
}