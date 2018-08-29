---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 0
info:
  title: CloudFlare Details about a specific Custom page details
  version: 1.0.0
  description: Details about a specific Custom page details
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /zones/:zone_identifier/custom_pages:
    get:
      summary: A list of available Custom Pages the zone can use
      description: A list of available Custom Pages the zone can use
      operationId: cloudflare-custom-pages-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-pages-get
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/:zone_identifier/custom_pages/:identifier:
    get:
      summary: Details about a specific Custom page details
      description: Details about a specific Custom page details
      operationId: cloudflare-custom-pages-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-pagesidentifier-get
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