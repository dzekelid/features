---
swagger: "2.0"
x-collection-name: Strava
x-complete: 0
info:
  title: Strava Get Activity Zones
  description: Premium Feature. Returns the zones of a given activity.
  version: 1.0.0
host: www.strava.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities/{id}/zones:
    get:
      summary: Get Activity Zones
      description: Premium Feature. Returns the zones of a given activity.
      operationId: getZonesByActivityId
      x-api-path-slug: activitiesidzones-get
      parameters:
      - in: path
        name: id
        description: The identifier of the activity
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Activity
      - Zones
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