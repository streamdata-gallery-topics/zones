---
swagger: "2.0"
x-collection-name: Data.Gov
info:
  title: Data.gov API Get Spatial Zones S
  description: Fetch a zone list as GeoJSON
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
  /spatial/zones/{ids}:
    get:
      summary: Get Spatial Zones S
      description: Fetch a zone list as GeoJSON
      operationId: getSpatialZonesS
      x-api-path-slug: spatialzonesids-get
      parameters:
      - in: path
        name: ids
        description: A zone identifiers list (comma separated)
      responses:
        200:
          description: OK
      tags:
      - Spatial
      - Zones
      - S
---