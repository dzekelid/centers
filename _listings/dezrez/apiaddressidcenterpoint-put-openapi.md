---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Update the Center Point for an Address
  version: 1.0.0
  description: Update the center point for an address.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/address/{id}/centerpoint:
    put:
      summary: Update the Center Point for an Address
      description: Update the center point for an address.
      operationId: Address_UpdateCenterPointByidByupdateCommand
      x-api-path-slug: apiaddressidcenterpoint-put
      parameters:
      - in: path
        name: id
        description: The Id of the address to update
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: updateCommand
        description: The point details which will be updated on the address
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Center
      - Pointan
      - Ress
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