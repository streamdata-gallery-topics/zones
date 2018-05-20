---
swagger: "2.0"
x-collection-name: AWS CloudHSM
info:
  title: AWS CloudHSM API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListAvailableZones:
    get:
      summary: List Available Zones
      description: Lists the Availability Zones that have available AWS CloudHSM capacity.
      operationId: listAvailableZones
      x-api-path-slug: actionlistavailablezones-get
      parameters:
      - in: query
        name: AZList
        description: The list of Availability Zones that have available AWS CloudHSM
          capacity
        type: string
      responses:
        200:
          description: OK
      tags:
      - Zones
---