---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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
---