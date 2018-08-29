swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeAvailabilityZones:
    get:
      summary: Describe Availability Zones
      description: Describes one or more of the Availability Zones that are available
        to you.
      operationId: describeavailabilityzones
      x-api-path-slug: actiondescribeavailabilityzones-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: RegionName.N
        description: The names of one or more regions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Availability Zones