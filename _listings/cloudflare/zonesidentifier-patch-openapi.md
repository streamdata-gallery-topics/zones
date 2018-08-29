---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 0
info:
  title: CloudFlare Only one zone property can be changed at a time
  version: 1.0.0
  description: Only one zone property can be changed at a time
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
  /zones/:zone_identifier/analytics/dashboard:
    get:
      summary: The dashboard view provides both totals and timeseries data for the
        given zone and time period across the entire CloudFlare network
      description: The dashboard view provides both totals and timeseries data for
        the given zone and time period across the entire CloudFlare network
      operationId: cloudflare-zone-analytics-api
      x-api-path-slug: zoneszone-identifieranalyticsdashboard-get
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
  /zones:
    get:
      summary: List, search, sort, and filter your zones
      description: List, search, sort, and filter your zones
      operationId: cloudflare-zone-api
      x-api-path-slug: zones-get
      parameters:
      - in: query
        name: direction
        description: Direction to order zonesttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: name
        description: A domain namettttttttttttttexample
      - in: query
        name: order
        description: Field to order zones byttttttttttttttstatus
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of zones per pagetttttttttttttt20
      - in: query
        name: status
        description: Status of the zonettttttttttttttactive
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
    post:
      summary: The domain name
      description: The domain name
      operationId: cloudflare-zone-api
      x-api-path-slug: zones-post
      parameters:
      - in: query
        name: name
        description: The domain namettttttttttttttexample
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
  /zones/:identifier:
    delete:
      summary: Delete an existing zone
      description: Delete an existing zone
      operationId: cloudflare-zone-api
      x-api-path-slug: zonesidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Zones
    get:
      summary: 'Zone details permission needed: #zone:read'
      description: 'Zone details permission needed: #zone:readntt'
      operationId: cloudflare-zone-api
      x-api-path-slug: zonesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Zones
    patch:
      summary: Only one zone property can be changed at a time
      description: Only one zone property can be changed at a time
      operationId: cloudflare-zone-api
      x-api-path-slug: zonesidentifier-patch
      parameters:
      - in: query
        name: paused
        description: Indicates if the zone is only using CloudFlare DNS services
      - in: query
        name: plan
        description: The desired plan for the zone
      - in: query
        name: vanity_name_servers
        description: An array of domains used for custom name servers
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