---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Access Control Retrieves connector configuration for external resource
    attributes for the given zone.
  description: Retrieves connector configuration for external resource attributes
    for the given zone..
  version: 1.0.0
host: predix-acs.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/connector/resource:
    get:
      summary: Retrieves connector configuration for external resource attributes
        for the given zone.
      description: Retrieves connector configuration for external resource attributes
        for the given zone..
      operationId: getResourceConnectorUsingGET_1
      x-api-path-slug: v1connectorresource-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Connector
      - Configurationexternal
      - Resource
      - Attributesthe
      - Given
      - Zone
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