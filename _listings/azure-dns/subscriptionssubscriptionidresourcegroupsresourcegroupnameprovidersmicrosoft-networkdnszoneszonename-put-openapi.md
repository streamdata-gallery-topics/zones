---
swagger: "2.0"
x-collection-name: Azure DNS
x-complete: 0
info:
  title: Azure DNS API Zones Create Or Update
  description: Creates or updates a DNS zone. Does not modify DNS records within the
    zone.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}:
    put:
      summary: Zones Create Or Update
      description: Creates or updates a DNS zone. Does not modify DNS records within
        the zone.
      operationId: Zones_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkdnszoneszonename-put
      parameters:
      - in: header
        name: If-Match
        description: The etag of the DNS zone
      - in: header
        name: If-None-Match
        description: Set to * to allow a new DNS zone to be created, but to prevent
          updating an existing zone
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to the CreateOrUpdate operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: zoneName
        description: The name of the DNS zone (without a terminating dot)
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