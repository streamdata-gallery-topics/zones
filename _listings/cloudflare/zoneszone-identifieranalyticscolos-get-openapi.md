---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 0
info:
  title: CloudFlare This view provides a breakdown of analytics data by datacenter
  version: 1.0.0
  description: This view provides a breakdown of analytics data by datacenter
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
    put:
      summary: Update Custom page URL
      description: Update Custom page URL
      operationId: cloudflare-custom-pages-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-pagesidentifier-put
      parameters:
      - in: query
        name: state
        description: The Custom Page statettttttttttttttdefault
      - in: query
        name: url
        description: A URL that is associated with the Custom Page
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/:zone_identifier/analytics/colos:
    get:
      summary: This view provides a breakdown of analytics data by datacenter
      description: This view provides a breakdown of analytics data by datacenter
      operationId: cloudflare-zone-analytics-api
      x-api-path-slug: zoneszone-identifieranalyticscolos-get
      parameters:
      - in: query
        name: continuous
        description: When set to true, the range returned by the response acts like
          a sliding window to provide a contiguous time-window
      - in: query
        name: since
        description: The (inclusive) beginning of the requested time frame
      - in: query
        name: until
        description: The (exclusive) end of the requested time frame
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Analytics
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