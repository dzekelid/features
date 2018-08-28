---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Add Reuses Reuse Featured
  description: Mark a reuse as featured
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /datasets/{dataset}/featured/:
    delete:
      summary: Delete Datasets Dataset Featured
      description: Unmark the dataset as featured
      operationId: deleteDatasetsDatasetFeatured
      x-api-path-slug: datasetsdatasetfeatured-delete
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Featured
    post:
      summary: Add Datasets Dataset Featured
      description: Mark the dataset as featured
      operationId: postDatasetsDatasetFeatured
      x-api-path-slug: datasetsdatasetfeatured-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Featured
  /reuses/{reuse}/featured/:
    delete:
      summary: Delete Reuses Reuse Featured
      description: Unmark a reuse as featured
      operationId: deleteReusesReuseFeatured
      x-api-path-slug: reusesreusefeatured-delete
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Featured
    post:
      summary: Add Reuses Reuse Featured
      description: Mark a reuse as featured
      operationId: postReusesReuseFeatured
      x-api-path-slug: reusesreusefeatured-post
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Featured
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