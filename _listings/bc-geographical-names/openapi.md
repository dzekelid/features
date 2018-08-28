swagger: "2.0"
x-collection-name: BC Geographical Names
x-complete: 1
info:
  title: Geo Mark Web Service
  description: the-geomark-web-service-allows-you-to-create-and-share-geographic-areas-of-interest-over-the-web-in-a-variety-of-formats-and-coordinate-systems--this-service-is-especially-helpful-when-you-need-to-share-an-area-of-interest-with-people-who-require-that-the-data-be-in-a-different-format-or-they-use-different-mapping-software-
  termsOfService: http://www2.gov.bc.ca/gov/content/governments/about-the-bc-government/databc/open-data/api-terms-of-use-for-ogl-information
  contact:
    name: Data BC
    url: http://data.gov.bc.ca/
    email: DataBCBA@gov.bc.ca
  version: 4.1.2
host: apps.gov.bc.ca
basePath: /pub/geomark
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /features/{featureId}:
    get:
      summary: Get a feature by its featureId
      description: Get information about the geographical feature with the specified
        featureId.
      operationId: get-information-about-the-geographical-feature-with-the-specified-featureid-
      x-api-path-slug: featuresfeatureid-get
      parameters:
      - in: path
        name: featureId
        description: The unique identifier for a feature
      responses:
        200:
          description: OK
      tags:
      - Features
      - FeatureId
  /featureCategories:
    get:
      summary: Get all feature categories
      description: 'Gets a list of all feature categories used by the BC Geographical
        Names Information System (BCGNIS).  Note: there are three levels of classification
        in the BCGNIS feature taxonomy: classes, categories and types.  A type is
        a subset of a category, and a category is a subset of a class.'
      operationId: gets-a-list-of-all-feature-categories-used-by-the-bc-geographical-names-information-system-bcgnis---
      x-api-path-slug: featurecategories-get
      parameters:
      - in: query
        name: outputFormat
        description: The format of the output
      responses:
        200:
          description: OK
      tags:
      - FeatureCategories
  /featureClasses:
    get:
      summary: Get all feature classes
      description: 'Gets a list of all feature classes used by the BC Geographical
        Names Information System (BCGNIS).  Note: there are three levels of classification
        in the BCGNIS feature taxonomy: classes, categories and types.  A type is
        a subset of a category, and a category is a subset of a class.'
      operationId: gets-a-list-of-all-feature-classes-used-by-the-bc-geographical-names-information-system-bcgnis---not
      x-api-path-slug: featureclasses-get
      parameters:
      - in: query
        name: outputFormat
        description: The format of the output
      responses:
        200:
          description: OK
      tags:
      - FeatureClasses
  /geomarks/{geomarkId}/feature.{fileFormatExtension}:
    get:
      summary: Get the feature and attribution of the geomark
      description: The geomark feature resource returns a single spatial feature with
        either a single (Point, LineString, Polygon) or multi-part geometry (MultiPoint,
        MultiLineString, MultiPolygon) and the geomark attribution.  The geometry
        and attribution can be downloaded as a spatial download file format in a supported
        coordinate system. The download files can then be used in a desktop GIS application
        (e.g. ArcMap), Google Earth or a web mapping application.
      operationId: the-geomark-feature-resource-returns-a-single-spatial-feature-with-either-a-single-point-linestring-
      x-api-path-slug: geomarksgeomarkidfeature-fileformatextension-get
      parameters:
      - in: path
        name: fileFormatExtension
        description: The file format name extension used to represent the geomark
          download
      - in: path
        name: geomarkId
        description: The unique identifier for the geomark (e
      - in: query
        name: srid
        description: The srid of the coordinate system the geometry should be converted
          to
      responses:
        200:
          description: OK
      tags:
      - Geomarks
      - GeomarkId
      - Feature
      - FileFormatExtension