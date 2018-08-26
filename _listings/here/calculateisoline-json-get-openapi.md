---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Routing API Time-based isoline with destination as center
  description: "*Request an isoline that will reach a destination within a given time*\n\nTime-based
    reverse flow requests are made using the `calculateisoline` endpoint and specifying
    the `destination` and `rangetype=time` parameters.\n\n\n\n* **mode**  `text`\n
    \\- Routing mode determines how the route is calculated.    e.g. `fastest;car;traffic:disabled.`\n\n*
    **destination**  `latlng`\n \\- Destination of the reverse flow calculation.    e.g.
    `52.515,13.377`\n\n* **rangetype**  `text`\n \\- Specifies type of range. Possible
    values are distance, time. For distance the unit is  meters. For time the unit
    is seconds.  rangetype=distance  rangetype=time    \n\n* **range**  `number`\n
    \\- Range of isoline. Several comma separated values can be specified. The unit
    is defined by  parameter rangetype  range=1000  range=1000,2000,3000  \n\n* **app_id**
    \ `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication
    of the client application.    You must include an `app_id` with every request.
    \ \n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used
    for the authentication of the client application.    You must include an `app_code`
    with every request."
  version: 1.0.0
host: route.cit.api.here.com
basePath: /routing/7.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calculateisoline.json:
    get:
      summary: Time-based isoline with destination as center
      description: "*Request an isoline that will reach a destination within a given
        time*\n\nTime-based reverse flow requests are made using the `calculateisoline`
        endpoint and specifying the `destination` and `rangetype=time` parameters.\n\n\n\n*
        **mode**  `text`\n \\- Routing mode determines how the route is calculated.
        \   e.g. `fastest;car;traffic:disabled.`\n\n* **destination**  `latlng`\n
        \\- Destination of the reverse flow calculation.    e.g. `52.515,13.377`\n\n*
        **rangetype**  `text`\n \\- Specifies type of range. Possible values are distance,
        time. For distance the unit is  meters. For time the unit is seconds.  rangetype=distance
        \ rangetype=time    \n\n* **range**  `number`\n \\- Range of isoline. Several
        comma separated values can be specified. The unit is defined by  parameter
        rangetype  range=1000  range=1000,2000,3000  \n\n* **app_id**  `text`\n \\-
        A 20 byte Base64 URL-safe encoded string used for the authentication of the
        client application.    You must include an `app_id` with every request.  \n\n*
        **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for
        the authentication of the client application.    You must include an `app_code`
        with every request."
      operationId: CalculateisolineJsonGet4
      x-api-path-slug: calculateisoline-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: destination
      - in: query
        name: mode
      - in: query
        name: range
      - in: query
        name: rangetype
      responses:
        200:
          description: OK
      tags:
      - Time-based
      - Isoline
      - Destination
      - As
      - Center
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