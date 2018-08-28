---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart Updates a specific feature from a specific Product
  version: 1.0.0
  description: Updates a specific feature from a specific product.
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Products/{catalogid}/Features:
    get:
      summary: Get the features from a specific Product
      description: Get the features from a specific product.
      operationId: Products_GetAllProductFeatures
      x-api-path-slug: 3dcartwebapiv1productscatalogidfeatures-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Features
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of features from a specific Product
      description: Updates a collection of features from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidfeatures-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: features
        description: A Json or XML object containing the new features
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Features
      - From
      - Specific
      - Product
    post:
      summary: Adds a new feature to the system
      description: Adds a new feature to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidfeatures-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: feature
        description: A Json or XML object containing the new feature
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Feature
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Features/{featureid}:
    put:
      summary: Updates a specific feature from a specific Product
      description: Updates a specific feature from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidfeaturesfeatureid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: feature
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: featureid
        description: FeatureID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Feature
      - From
      - Specific
      - Product
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