---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Intelligent Mapping Return collection features in specified bounding
    box
  description: |-
    Returns all features in the specified collection that exist fully or
    partially within the specified bounding box. The bounding box is defined
    by two coordinates in the EPSG:4326 (WGS84) (for further details see
    http://epsg.io/4326):

    * left (longitude), bottom (latitude)

    * right (longitude), top (latitude)
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/collections/{collectionName}/spatial-query/bbox-interacts:
    get:
      summary: Return collection features in specified bounding box
      description: |-
        Returns all features in the specified collection that exist fully or
        partially within the specified bounding box. The bounding box is defined
        by two coordinates in the EPSG:4326 (WGS84) (for further details see
        http://epsg.io/4326):

        * left (longitude), bottom (latitude)

        * right (longitude), top (latitude)
      operationId: returns-all-features-in-the-specified-collection-that-exist-fully-orpartially-within-the-specified-b
      x-api-path-slug: v1collectionscollectionnamespatialquerybboxinteracts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Return
      - Collection
      - Features
      - In
      - Specified
      - Bounding
      - Box
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