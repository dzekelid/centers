swagger: "2.0"
x-collection-name: Fire Browse
x-complete: 1
info:
  title: Fire Browse Beta API
  description: a-simple-and-elegant-way-to-explore-cancer-data
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
  /Metadata/Centers:
    get:
      summary: Obtain identities of TCGA consortium member centers.
      description: By default this function returns a table of all consortium members
        in TCGA, aka centers; it provides both the HTTP domain and full organizational
        name of each center.  A subset of this table may be obtained by explicitly
        specifying one or more domain names.
      operationId: getMetadataCenters
      x-api-path-slug: metadatacenters-get
      parameters:
      - in: query
        name: center
        description: Narrow search to one or more TCGA centers from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Centers