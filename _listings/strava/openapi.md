swagger: "2.0"
x-collection-name: Strava
x-complete: 1
info:
  title: Strava API v3
  description: strava-api
  version: 1.0.0
host: www.strava.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /athlete/zones:
    get:
      summary: Get Zones
      description: Returns the the authenticated athlete's heart rate and power zones.
      operationId: getLoggedInAthleteZones
      x-api-path-slug: athletezones-get
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Zones
  /activities/{id}/zones:
    get:
      summary: Get Activity Zones
      description: Premium Feature. Returns the zones of a given activity.
      operationId: getZonesByActivityId
      x-api-path-slug: activitiesidzones-get
      parameters:
      - in: path
        name: id
        description: The identifier of the activity
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Activity
      - Zones