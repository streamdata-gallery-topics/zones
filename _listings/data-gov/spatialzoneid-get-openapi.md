---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Get Spatial Zone
  description: Fetch a zone
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /spatial/zone/{id}:
    get:
      summary: Get Spatial Zone
      description: Fetch a zone
      operationId: getSpatialZone
      x-api-path-slug: spatialzoneid-get
      parameters:
      - in: path
        name: id
        description: A zone identifier
      responses:
        200:
          description: OK
      tags:
      - Spatial
      - Zone
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