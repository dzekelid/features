---
swagger: "2.0"
x-collection-name: Codefresh
x-complete: 0
info:
  title: Codefresh Get Features Accountid
  description: Get features accountid.
  termsOfService: http://www.codefresh.io
  contact:
    name: Codefresh api team
    url: http://www.codefresh.io
  version: 1.0.0
host: g.codefresh.io
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /features/{accountId}:
    get:
      summary: Get Features Accountid
      description: Get features accountid.
      operationId: getFeaturesAccount
      x-api-path-slug: featuresaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account to query for feature availability
      responses:
        200:
          description: OK
      tags:
      - Features
      - Accountid
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