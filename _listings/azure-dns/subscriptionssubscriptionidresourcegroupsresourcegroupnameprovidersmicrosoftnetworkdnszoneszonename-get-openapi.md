---
swagger: "2.0"
info:
  title: Azure DNS API Zones Get
  description: Gets a DNS zone. Retrieves the zone properties, but not the record
    sets within the zone.
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
      parameters:
      - in: header
        name: If-Match
        description: The etag of the DNS zone
      - in: header
        name: If-None-Match
        description: Set to '*' to allow a new DNS zone to be created, but to prevent
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
    delete:
      summary: Zones Delete
      description: 'Deletes a DNS zone. WARNING: All DNS records in the zone will
        also be deleted. This operation cannot be undone.'
      operationId: Zones_Delete
      parameters:
      - in: header
        name: If-Match
        description: The etag of the DNS zone
      - in: query
        name: No Name
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
    get:
      summary: Zones Get
      description: Gets a DNS zone. Retrieves the zone properties, but not the record
        sets within the zone.
      operationId: Zones_Get
      parameters:
      - in: query
        name: No Name
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
---