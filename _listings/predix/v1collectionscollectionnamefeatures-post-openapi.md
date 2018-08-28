---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Intelligent Mapping Insert an individual feature into a collection.
  description: |-
    Insert a new feature into the the named collection. The GeoJSON id is used to identify the feature.
    The GeoJSON id included in the url must match the top level id member of the feature provided.
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
  /v1/collections/{collectionName}/features:
    delete:
      summary: Delete from the named collection all features with a matching GeoJSON
        id.
      description: Delete from the named collection all features with a matching GeoJSON
        id. This could be 0, 1 or many features.
      operationId: delete-from-the-named-collection-all-features-with-a-matching-geojson-id-this-could-be-0-1-or-many-f
      x-api-path-slug: v1collectionscollectionnamefeatures-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - From
      - Named
      - Collection
      - ""
      - Features
      - Matching
      - GeoJSON
      - Id
    put:
      summary: Update all features in a collection with a matching GeoJSON id.
      description: Updates the attributes and geometry of matching features in the
        named collection.  This could be 0, 1 or many features.
      operationId: updates-the-attributes-and-geometry-of-matching-features-in-the-named-collection--this-could-be-0-1-
      x-api-path-slug: v1collectionscollectionnamefeatures-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Features
      - In
      - Collection
      - Matching
      - GeoJSON
      - Id
    get:
      summary: Return feature
      description: |-
        Returns GeoJSON of type FeatureCollection containing all GeoJSON features
        from the named collection with a matching GeoJSON id.
      operationId: returns-geojson-of-type-featurecollection-containing-all-geojson-featuresfrom-the-named-collection-w
      x-api-path-slug: v1collectionscollectionnamefeatures-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Return
      - Feature
    post:
      summary: Insert an individual feature into a collection.
      description: |-
        Insert a new feature into the the named collection. The GeoJSON id is used to identify the feature.
        The GeoJSON id included in the url must match the top level id member of the feature provided.
      operationId: insert-a-new-feature-into-the-the-named-collection-the-geojson-id-is-used-to-identify-the-featurethe
      x-api-path-slug: v1collectionscollectionnamefeatures-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Individual
      - Feature
      - Into
      - Collection
  /v1/collections/{collectionName}/cluster:
    get:
      summary: Returns clustering data for collection features in specified bounding
        box
      description: |-
        Returns Clustering data for the specified collection that exist fully
         or partially within the specified bounding box. The bounding box is
         defined by two coordinates in the EPSG:4326 (WGS84)
         (for further details see http://epsg.io/4326):
         * left (longitude), bottom (latitude)
         * right (longitude), top (latitude)
      operationId: returns-clustering-data-for-the-specified-collection-that-exist-fully-or-partially-within-the-specif
      x-api-path-slug: v1collectionscollectionnamecluster-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Clustering
      - Datacollection
      - Features
      - In
      - Specified
      - Bounding
      - Box
  /v1/collections/{collectionName}/text:
    get:
      summary: Free text search of a feature collection
      description: |-
        Returns GeoJSON of type FeatureCollection containing all GeoJSON features from the named collection that match
        the supplied search string.

        The search text consists of one or more strings that can be space or comma separated. A match with a given
        feature occurs only if an exact match can be found for each of the strings in the search text amongst a
        concatenation of the values of child members of the top level 'properties' member of the feature,
        together with the value of its GeoJSON id. The matching is case insensitve, partial matches and
        wildcard searching is not supported.

        Examples of search text:

         - 28,West End,Histon
         - 240.000 V
         - Company Owned
      operationId: returns-geojson-of-type-featurecollection-containing-all-geojson-features-from-the-named-collection-
      x-api-path-slug: v1collectionscollectionnametext-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: q
        description: The search text
      responses:
        200:
          description: OK
      tags:
      - Free
      - Text
      - Search
      - Of
      - Feature
      - Collection
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