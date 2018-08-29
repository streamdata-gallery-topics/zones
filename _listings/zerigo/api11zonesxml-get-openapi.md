---
swagger: "2.0"
x-collection-name: Zerigo
x-complete: 0
info:
  title: Zerigo List all zones
  version: 1.0.0
  description: 'There are two optional parameters: page=# and per_page=#. page defaults
    to 1 (and starts at 1, not 0). per_page defaults to 100 but should be specified
    exactly if a change of the default value will cause your application to fail.
    The maximum value for per_page is 1000.'
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/1.1/zones.xml:
    get:
      summary: List all zones
      description: 'There are two optional parameters: page=# and per_page=#. page
        defaults to 1 (and starts at 1, not 0). per_page defaults to 100 but should
        be specified exactly if a change of the default value will cause your application
        to fail. The maximum value for per_page is 1000.'
      operationId: list-all-zones
      x-api-path-slug: api11zonesxml-get
      responses:
        200:
          description: OK
      tags:
      - Zones
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