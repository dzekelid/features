{
  "info": {
    "name": "Botify Get Analyses Username Project Slug Analysis Slug Features Ganalytics Orphan Urls Medium Source",
    "_postman_id": "3fbe9624-24bf-45cb-84cd-cbc5168d365f",
    "description": "Legacy    List of Orphan URLs. URLs which generated visits from the selected source according to Google Analytics data, but were not crawled with by the Botify crawler (either because no links to them were found on the website, or because the crawler was not allowed to follow these links according to the project settings).   For a search engine (medium: origanic; sources: all, aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social network (medium: social; sources: all, facebook, google+, linkedin, pinterest, reddit, tumblr, twitter)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analyses",
      "item": [
        {
          "id": "80ee082a-3166-4883-97f5-7cee321fe053",
          "name": "getAnalysesUsernameProjectSlugAnalysisSlugFeaturesGanalyticsOrphanUrlsMediumSource",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.botify.com",
              "path": [
                "v1",
                "analyses/:username/:project_slug/:analysis_slug/features/ganalytics/orphan_urls/:medium/:source"
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
            "description": "Legacy    List of Orphan URLs. URLs which generated visits from the selected source according to Google Analytics data, but were not crawled with by the Botify crawler (either because no links to them were found on the website, or because the crawler was not allowed to follow these links according to the project settings).   For a search engine (medium: origanic; sources: all, aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social network (medium: social; sources: all, facebook, google+, linkedin, pinterest, reddit, tumblr, twitter)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35eaab73-d081-4e5f-8fdd-d6496778767a"
            }
          ]
        }
      ]
    }
  ]
}