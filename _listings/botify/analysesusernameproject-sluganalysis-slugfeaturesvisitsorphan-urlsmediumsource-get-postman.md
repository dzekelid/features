{
  "info": {
    "name": "Botify Get Analyses Username Project Slug Analysis Slug Features Visits Orphan Urls Medium Source",
    "_postman_id": "e9e50ae8-2f79-40ee-84e7-f4978e22067c",
    "description": "List of Orphan URLs. URLs which generated visits from the selected source according to Google Analytics data, but were not crawled with by the Botify crawler (either because no links to them were found on the website, or because the crawler was not allowed to follow these links according to the project settings).   For a search engine (medium: origanic; sources: all, aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social network (medium: social; sources: all, facebook, google+, linkedin, pinterest, reddit, tumblr, twitter)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analyses",
      "item": [
        {
          "id": "6fef704b-d353-49ba-8db3-e9fd541f0cc7",
          "name": "getAnalysesUsernameProjectSlugAnalysisSlugFeaturesVisitsOrphanUrlsMediumSource",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.botify.com",
              "path": [
                "v1",
                "analyses/:username/:project_slug/:analysis_slug/features/visits/orphan_urls/:medium/:source"
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
                },
                {
                  "id": "medium",
                  "value": "medium",
                  "type": "string"
                },
                {
                  "id": "source",
                  "value": "source",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of Orphan URLs. URLs which generated visits from the selected source according to Google Analytics data, but were not crawled with by the Botify crawler (either because no links to them were found on the website, or because the crawler was not allowed to follow these links according to the project settings).   For a search engine (medium: origanic; sources: all, aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social network (medium: social; sources: all, facebook, google+, linkedin, pinterest, reddit, tumblr, twitter)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29d67004-6df3-46c6-a98e-cf279d28a9ed"
            }
          ]
        }
      ]
    }
  ]
}