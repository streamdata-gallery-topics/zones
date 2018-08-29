swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /zones:
    get:
      summary: Get Zones
      description: Returns zones.
      operationId: FindZones
      x-api-path-slug: zones-get
      parameters:
      - in: query
        name: applianceUri
        description: The appliance URI to prune zones by
      - in: query
        name: providerUri
        description: The provider URI to prune zones by
      - in: query
        name: query
        description: Filters the zones returned
      - in: query
        name: regionUri
        description: The region URI to prune zones by
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Include all the details
          of the zones'
      responses:
        200:
          description: OK
      tags:
      - Zones
    post:
      summary: Post Zones
      description: Creates a new zone
      operationId: CreateZone
      x-api-path-slug: zones-post
      parameters:
      - in: body
        name: zone
        description: Add new zone
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/{id}:
    delete:
      summary: Delete Zones
      description: Deletes a zone
      operationId: DeleteZone
      x-api-path-slug: zonesid-delete
      parameters:
      - in: query
        name: force
        description: Zones may be in an odd state
      - in: path
        name: id
        description: ID of zone to delete
      responses:
        200:
          description: OK
      tags:
      - Zones
    get:
      summary: Get Zones
      description: Returns a zone based on its id.
      operationId: GetZoneById
      x-api-path-slug: zonesid-get
      parameters:
      - in: path
        name: id
        description: ID of zone to fetch
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Zones
    patch:
      summary: Patch Zones
      description: Updates a zone
      operationId: UpdateZone
      x-api-path-slug: zonesid-patch
      parameters:
      - in: path
        name: id
        description: ID of zone to update
      - in: body
        name: zone
        description: Update zone
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/{id}/actions:
    post:
      summary: Post Zones Actions
      description: Peforms an action to the zone. It requires the **administrator**
        role.
      operationId: ActOnZone
      x-api-path-slug: zonesidactions-post
      parameters:
      - in: body
        name: action
        description: Action to perform
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of zone to act on
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Actions
  /zones/{id}/appliance-image:
    get:
      summary: Get Zones Appliance Image
      description: Generates appliance-image url for the zone
      operationId: appliance-image
      x-api-path-slug: zonesidapplianceimage-get
      parameters:
      - in: path
        name: id
        description: ID of zone to fetch the appliance-image
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Appliance
      - Image
  /zones/{id}/connections:
    get:
      summary: Get Zones Connections
      description: Gets the list of connection for the zone. It requires the **administrator**
        role.
      operationId: zoneConnectionInstances
      x-api-path-slug: zonesidconnections-get
      parameters:
      - in: path
        name: id
        description: ID of zone to fetch the list of connection for the zone
      - in: query
        name: uuid
        description: Type to filter connection by
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Connections
    post:
      summary: Post Zones Connections
      description: Peforms an action to the zone. It requires the **administrator**
        role.
      operationId: RegisterZoneConnection
      x-api-path-slug: zonesidconnections-post
      parameters:
      - in: path
        name: id
        description: ID of zone to act on
      - in: body
        name: zoneConnection
        description: Create a new connection instance for the zone
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Connections
  /zones/{id}/connections/{uuid}:
    delete:
      summary: Delete Zones Connections Uu
      description: Deletes a connection instance of the zone
      operationId: UnregisterZoneConnection
      x-api-path-slug: zonesidconnectionsuuid-delete
      parameters:
      - in: path
        name: id
        description: ID of zone
      - in: path
        name: uuid
        description: ID of connection
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Connections
      - Uu
    patch:
      summary: Patch Zones Connections Uu
      description: Updates a connection of the zone.
      operationId: UpdateZoneConnection
      x-api-path-slug: zonesidconnectionsuuid-patch
      parameters:
      - in: path
        name: id
        description: ID of zone
      - in: path
        name: uuid
        description: ID of connection
      - in: body
        name: zoneConnection
        description: Update connection
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Connections
      - Uu
  /zones/{id}/task-status:
    get:
      summary: Get Zones Task Status
      description: Returns the status of the task for the zone
      operationId: ZoneTaskStatus
      x-api-path-slug: zonesidtaskstatus-get
      parameters:
      - in: path
        name: id
        description: ID of zone to fetch the task details
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Task
      - Status