---
swagger: "2.0"
info:
  title: AWS Route 53 API Get Hosted Zone
  version: 1.0.0
  description: Retrieves the delegation set for a hosted zone, including the four
    name serversassigned to the hosted zone. Send a GET request to the /Amazon Route
    53 APIversion/hostedzone/hosted zone ID             resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/hostedzone/Id:
    get:
      summary: Get Hosted Zone
      description: Retrieves the delegation set for a hosted zone, including the four
        name serversassigned to the hosted zone
      operationId: gethostedzone
      parameters:
      - in: path
        name: Id
        description: "The ID of the hosted zone for which you want to get a list of
          the name servers in the\t\t\tdelegation set"
        type: string
      responses:
        200:
          description: OK
      tags:
      - hosted zones
definitions: []
x-collection-name: AWS Route 53
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