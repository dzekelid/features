---
name: Predix
x-slug: predix
description: Predix (IoT PaaS) helps you develop apps that connect people with industrial
  machines through analytics and data for better business outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
x-kinRank: "7"
x-alexaRank: "264121"
tags: Features
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/apis.md
specificationVersion: "0.14"
apis:
- name: Intelligent Mapping - Return collection features in specified bounding box
  x-api-slug: v1collectionscollectionnamespatialquerybboxinteracts-get
  description: |-
    Returns all features in the specified collection that exist fully or
    partially within the specified bounding box. The bounding box is defined
    by two coordinates in the EPSG:4326 (WGS84) (for further details see
    http://epsg.io/4326):

    * left (longitude), bottom (latitude)

    * right (longitude), top (latitude)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnamespatialquerybboxinteracts-get-openapi.md
- name: Intelligent Mapping - Delete from the named collection all features with a
    matching GeoJSON id.
  x-api-slug: v1collectionscollectionnamefeatures-delete
  description: Delete from the named collection all features with a matching GeoJSON
    id. This could be 0, 1 or many features.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnamefeatures-delete-openapi.md
- name: Intelligent Mapping - Update all features in a collection with a matching
    GeoJSON id.
  x-api-slug: v1collectionscollectionnamefeatures-put
  description: Updates the attributes and geometry of matching features in the named
    collection.  This could be 0, 1 or many features.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnamefeatures-put-openapi.md
- name: Intelligent Mapping - Returns clustering data for collection features in specified
    bounding box
  x-api-slug: v1collectionscollectionnamecluster-get
  description: |-
    Returns Clustering data for the specified collection that exist fully
     or partially within the specified bounding box. The bounding box is
     defined by two coordinates in the EPSG:4326 (WGS84)
     (for further details see http://epsg.io/4326):
     * left (longitude), bottom (latitude)
     * right (longitude), top (latitude)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnamecluster-get-openapi.md
- name: Intelligent Mapping - Return feature
  x-api-slug: v1collectionscollectionnamefeatures-get
  description: |-
    Returns GeoJSON of type FeatureCollection containing all GeoJSON features
    from the named collection with a matching GeoJSON id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnamefeatures-get-openapi.md
- name: Intelligent Mapping - Insert an individual feature into a collection.
  x-api-slug: v1collectionscollectionnamefeatures-post
  description: |-
    Insert a new feature into the the named collection. The GeoJSON id is used to identify the feature.
    The GeoJSON id included in the url must match the top level id member of the feature provided.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnamefeatures-post-openapi.md
- name: Intelligent Mapping - Free text search of a feature collection
  x-api-slug: v1collectionscollectionnametext-get
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnametext-get-openapi.md
- name: Intelligent Mapping - Return feature
  x-api-slug: v1collectionscollectionnamefeatures-get
  description: |-
    Returns GeoJSON of type FeatureCollection containing all GeoJSON features
    from the named collection with a matching GeoJSON id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnamefeatures-get-openapi.md
- name: Intelligent Mapping - Insert an individual feature into a collection.
  x-api-slug: v1collectionscollectionnamefeatures-post
  description: |-
    Insert a new feature into the the named collection. The GeoJSON id is used to identify the feature.
    The GeoJSON id included in the url must match the top level id member of the feature provided.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnamefeatures-post-openapi.md
- name: Intelligent Mapping - Free text search of a feature collection
  x-api-slug: v1collectionscollectionnametext-get
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnametext-get-openapi.md
- name: Intelligent Mapping - Free text search of a feature collection
  x-api-slug: v1collectionscollectionnametext-get
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnametext-get-openapi.md
- name: Intelligent Mapping - Insert an individual feature into a collection.
  x-api-slug: v1collectionscollectionnamefeatures-post
  description: |-
    Insert a new feature into the the named collection. The GeoJSON id is used to identify the feature.
    The GeoJSON id included in the url must match the top level id member of the feature provided.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnamefeatures-post-openapi.md
- name: Intelligent Mapping - Return feature
  x-api-slug: v1collectionscollectionnamefeatures-get
  description: |-
    Returns GeoJSON of type FeatureCollection containing all GeoJSON features
    from the named collection with a matching GeoJSON id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/predix/v1collectionscollectionnamefeatures-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://predicthq.api.gallery.streamdata.io
- type: x-api-stack
  url: http://predix.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/predix
- type: x-documentation
  url: https://docs.predix.io/en-US/platform
- type: x-twitter
  url: https://twitter.com/Predix
- type: x-website
  url: https://www.predix.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---