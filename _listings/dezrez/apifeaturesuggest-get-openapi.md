---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get feature suggestions for value
  version: 1.0.0
  description: Get feature suggestions for value.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/feature/list:
    get:
      summary: Get  a list of features by a list of ids
      description: Get  a list of features by a list of ids.
      operationId: Feature_GetByfeatureid
      x-api-path-slug: apifeaturelist-get
      parameters:
      - in: query
        name: featureid
        description: the list of ids
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Features
      - By
      - List
      - Of
      - Ids
  /api/feature/{name}:
    get:
      summary: Get a feature by its name
      description: Get a feature by its name.
      operationId: Feature_GetByname
      x-api-path-slug: apifeaturename-get
      parameters:
      - in: path
        name: name
        description: The name of the feature to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Feature
      - By
      - Its
      - Name
  /api/feature/suggest:
    get:
      summary: Get feature suggestions for value
      description: Get feature suggestions for value.
      operationId: Feature_SuggestByname
      x-api-path-slug: apifeaturesuggest-get
      parameters:
      - in: query
        name: name
        description: The value to retrieve suggestions for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Feature
      - Suggestionsvalue
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---