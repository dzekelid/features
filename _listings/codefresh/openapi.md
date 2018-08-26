---
swagger: "2.0"
x-collection-name: Codefresh
x-complete: 1
info:
  title: Codefresh API
  description: codefresh-api-swagger2-0-specification
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
---