---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: 'Dezrez '
  version: 1.0.0
  description: .
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
  /api/featureprovisioning/enrollagency:
    post:
      summary: Enrolls an agency into a feature
      description: Enrolls an agency into a feature.
      operationId: FeatureProvisioning_EnrollAgencyInFeatureByfeatureSystemName
      x-api-path-slug: apifeatureprovisioningenrollagency-post
      parameters:
      - in: query
        name: featureSystemName
        description: The SystemName of the feature
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Enrolls
      - Agency
      - Into
      - Feature
  /api/admin/system/CreateNewSystemFeature:
    post:
      summary: Creates a new system wide feature available for activation.
      description: Creates a new system wide feature available for activation..
      operationId: System_CreateNewSystemFeatureBysaveNewFeatureCommad
      x-api-path-slug: apiadminsystemcreatenewsystemfeature-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: saveNewFeatureCommad
        description: The save new feature commad
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - System
      - Wide
      - Feature
      - Availableactivation
  /api/enlistedfeature/getvalidforagency:
    get:
      summary: Gets all the active features for an agency
      description: Gets all the active features for an agency.
      operationId: EnlistedFeature_GetAllValidEnlistedFeaturesForAgency
      x-api-path-slug: apienlistedfeaturegetvalidforagency-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Active
      - Featuresan
      - Agency
  /api/FeatureDescription/{id}:
    get:
      summary: ""
      description: .
      operationId: FeatureDescription_GetByid
      x-api-path-slug: apifeaturedescriptionid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - ""
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