---
swagger: "2.0"
x-collection-name: Zerigo
x-complete: 0
info:
  title: Zerigo Create a zone
  version: 1.0.0
  description: ns1 should be left out unless ns-type is &#8216;sec&#8217;. slave-nameservers
    should be left out unless ns-type is &#8216;pri&#8217;. See more details under
    Zones Overview.
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
    post:
      summary: Create a zone
      description: ns1 should be left out unless ns-type is &#8216;sec&#8217;. slave-nameservers
        should be left out unless ns-type is &#8216;pri&#8217;. See more details under
        Zones Overview.
      operationId: create-a-zone
      x-api-path-slug: api11zonesxml-post
      responses:
        200:
          description: OK
      tags:
      - Zones
  header:
    x-query-count:
      summary: Count all zones
      description: This is the total number of zones available. It is the same value
        as provided in the X-Query-Count header in the Managed DNS &#8594; List all
        zones API method.
      operationId: count-all-zones
      x-api-path-slug: header-xquerycount
      responses:
        200:
          description: OK
      tags:
      - Zones
  and:
    hosts-count:
      summary: Get a zone
      description: This response is similar to Listing All Zones, with the addition
        of hosts-count and possibly hosts. As long as there are no more than 300 hosts,
        they will be returned. If there are more, the hosts array will be left out.
        hosts-count will always be returned.
      operationId: get-a-zone
      x-api-path-slug: and-hostscount
      responses:
        200:
          description: OK
      tags:
      - Zones
  /api/1.1/zones/12345678/stats.xml:
    get:
      summary: Get stats for a zone
      description: This response returns current traffic statistics about this zone.
        Queries is measured from the beginning of the current period through the time
        of the API call. Just like everywhere else in our system, dates are based
        on UTC.
      operationId: get-stats-for-a-zone
      x-api-path-slug: api11zones12345678statsxml-get
      responses:
        200:
          description: OK
      tags:
      - Zones
  /api/1.1/zones/new.xml:
    get:
      summary: Get a blank zone
      description: This response may be useful to obtain a blank zone, suitable for
        use as a template or retrieving default values for included fields.
      operationId: get-a-blank-zone
      x-api-path-slug: api11zonesnewxml-get
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