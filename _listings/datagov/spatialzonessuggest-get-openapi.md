---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Get Spatial Zones Suggest
  description: Suggest geospatial zones
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
  /spatial/zones/suggest:
    get:
      summary: Get Spatial Zones Suggest
      description: Suggest geospatial zones
      operationId: getSpatialZonesSuggest
      x-api-path-slug: spatialzonessuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Spatial
      - Zones
      - Suggest
---