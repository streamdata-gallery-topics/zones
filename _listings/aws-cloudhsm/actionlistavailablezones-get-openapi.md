---
swagger: "2.0"
x-collection-name: AWS CloudHSM
x-complete: 0
info:
  title: AWS CloudHSM API List Available Zones
  version: 1.0.0
  description: Lists the Availability Zones that have available AWS CloudHSM capacity.
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