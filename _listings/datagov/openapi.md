---
swagger: "2.0"
x-collection-name: Data.Gov
info:
  title: Data.gov API
  description: the-datagov-catalog-is-powered-by-ckan-a-powerful-open-source-data-platform-that-includes-a-robust-api-please-be-aware-that-datagov-and-the-datagov-ckan-api-only-contain-metadata-about-datasets-this-metadata-includes-urls-and-descriptions-of-datasets-but-it-does-not-include-the-actual-data-within-each-dataset
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