swagger: "2.0"
x-collection-name: Google Compute Engine
x-complete: 1
info:
  title: Compute Engine
  description: creates-and-runs-virtual-machines-on-google-cloud-platform-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/zones:
    get:
      summary: Get Zones
      description: Retrieves the list of Zone resources available to the specified
        project.
      operationId: compute.zones.list
      x-api-path-slug: projectzones-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Zone
  /{project}/zones/{zone}:
    get:
      summary: Get Zone
      description: Returns the specified Zone resource. Get a list of available zones
        by making a list() request.
      operationId: compute.zones.get
      x-api-path-slug: projectzoneszone-get
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: Name of the zone resource to return
      responses:
        200:
          description: OK
      tags:
      - Zone