swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 1
info:
  title: Data.gov API
  description: the-data-gov-catalog-is-powered-by-ckan-a-powerful-open-source-data-platform-that-includes-a-robust-api--please-be-aware-that-data-gov-and-the-data-gov-ckan-api-only-contain-metadata-about-datasets--this-metadata-includes-urls-and-descriptions-of-datasets-but-it-does-not-include-the-actual-data-within-each-dataset-
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