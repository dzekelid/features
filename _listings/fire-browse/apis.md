---
name: Fire Browse
x-slug: fire-browse
description: A simple and elegant way to explore cancer data. Sitting above one of
  the deepest and most integratively characterized open cancer datasets in the world.
  Backed by a powerful computational infrastructure, application programming interface
  (API), graphical tools and online reports. With over 80K sample aliquots from 11,000+
  cancer patients, spanning 38 unique disease cohorts.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Features
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/fire-browse/apis.md
specificationVersion: "0.14"
apis:
- name: Fire Browse Beta API - Retrieve aggregated analysis features table.
  x-api-slug: analysesfeaturetable-get
  description: This service returns part or all of the so-called feature table; which
    aggregates the most important findings across ALL pipelines in the GDAC Firehose
    analysis workflow into a single table for simple access.  One feature table is
    created per disease cohort.  Results may be filtered by date or cohort, but at
    least 1 cohort must be specified here. For more details please visit the online
    documentation.  Please note that the service is still undergoing experimental
    evaluation and does not return JSON format.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1
  tags: Cancer, API Provider, Data Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/fire-browse/analysesfeaturetable-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/features/master/_listings/fire-browse/analysesfeaturetable-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://factual.api.gallery.streamdata.io
- type: x-api-stack
  url: http://fire.browse.stack.network
- type: x-website
  url: http://firebrowse.org
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---