---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Get Articles Featured
  description: See featured Reverb blog posts
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /articles/featured:
    get:
      summary: Get Articles Featured
      description: See featured Reverb blog posts
      operationId: getArticlesFeatured
      x-api-path-slug: articlesfeatured-get
      responses:
        200:
          description: OK
      tags:
      - Articles
      - Featured
  /articles/recently_featured:
    get:
      summary: Get Articles Recently Featured
      description: Get articles recently featured.
      operationId: getArticlesRecentlyFeatured
      x-api-path-slug: articlesrecently-featured-get
      responses:
        200:
          description: OK
      tags:
      - Articles
      - Recently
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