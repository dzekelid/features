---
swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 1
info:
  title: IDX API 1.4.0 Test Runner
  description: idx-broker-api-calls-in-version-1-4-0required-environment-variable-url-environment-variable-for-request-headers-environment-variable-partner-key-client-account-with-at-least-one-featured-listingtests-are-in-this-order-as-variables-such-as-listing-id-and-approved-mls-are-passed-to-subsequent-api-calls-
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /clients/featured:
    get:
      summary: Get Featured
      description: Returns a basic set of information for all of the client's featured
        (active) properties
      operationId: ClientsFeaturedGet
      x-api-path-slug: clientsfeatured-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Featured
  /clients/listallowedfields/{approvedMLS}/{featuredId}:
    get:
      summary: Get List Allowed Fields Approved MLS Featured
      description: Returns the allowed returnable fields for a given listingID.
      operationId: ClientsListallowedfieldsByApprovedMLSAndFeaturedIdGet
      x-api-path-slug: clientslistallowedfieldsapprovedmlsfeaturedid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: path
        name: featuredId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - List
      - Owed
      - Fields
      - Approved
      - MLS
      - Featured
  /partners/aggregatedfeatured:
    get:
      summary: Get Partners Aggregated Featured
      description: Get a list of featured MLS properties.
      operationId: PartnersAggregatedfeaturedGet
      x-api-path-slug: partnersaggregatedfeatured-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Featured
  /clients/listing/{approvedMLS}/{featuredId}:
    get:
      summary: Get Listing Approved MLS Featuredid
      description: Returns the detailed information for a given listingID.
      operationId: ClientsListingByApprovedMLSAndFeaturedIdGet
      x-api-path-slug: clientslistingapprovedmlsfeaturedid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: path
        name: featuredId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Approved
      - MLS
      - Featuredid
---