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
tags: Centers
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/centers/master/_listings/fire-browse/apis.md
specificationVersion: "0.14"
apis:
- name: Fire Browse Beta API - Obtain identities of TCGA consortium member centers.
  x-api-slug: metadatacenters-get
  description: By default this function returns a table of all consortium members
    in TCGA, aka centers; it provides both the HTTP domain and full organizational
    name of each center.  A subset of this table may be obtained by explicitly specifying
    one or more domain names.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1
  tags: Cancer, API Provider, Data Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/centers/master/_listings/fire-browse/metadatacenters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/centers/master/_listings/fire-browse/metadatacenters-get-openapi.md
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