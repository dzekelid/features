---
swagger: "2.0"
x-collection-name: Fire Browse
x-complete: 0
info:
  title: Fire Browse Beta API Retrieve aggregated analysis features table.
  description: This service returns part or all of the so-called feature table; which
    aggregates the most important findings across ALL pipelines in the GDAC Firehose
    analysis workflow into a single table for simple access.  One feature table is
    created per disease cohort.  Results may be filtered by date or cohort, but at
    least 1 cohort must be specified here. For more details please visit the online
    documentation.  Please note that the service is still undergoing experimental
    evaluation and does not return JSON format.
  version: 1.1.35 (2016-09-27 10:12:23 6a47e74011281b2aa
host: firebrowse.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Analyses/FeatureTable:
    get:
      summary: Retrieve aggregated analysis features table.
      description: This service returns part or all of the so-called feature table;
        which aggregates the most important findings across ALL pipelines in the GDAC
        Firehose analysis workflow into a single table for simple access.  One feature
        table is created per disease cohort.  Results may be filtered by date or cohort,
        but at least 1 cohort must be specified here. For more details please visit
        the online documentation.  Please note that the service is still undergoing
        experimental evaluation and does not return JSON format.
      operationId: getAnalysesFeaturetable
      x-api-path-slug: analysesfeaturetable-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: column
        description: Comma separated list of which data columns/fields to return
      - in: query
        name: date
        description: Select one or more date stamps
      - in: query
        name: format
        description: Format of result
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - FeatureTable
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