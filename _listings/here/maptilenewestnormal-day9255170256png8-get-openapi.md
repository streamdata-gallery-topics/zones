---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Map Tile API Toll Zone Map
  description: |-
    *Request a street map tile highlighting congestion and environmental toll zones*

    To highlight such toll zones, add the `congestion` parameter to the request URL.



    * **congestion**  `null`
     \- Flag to indicate if congestion zones are to be shown on the map.

    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
  version: 1.0.0
host: 1.aerial.maps.cit.api.here.com
basePath: /maptile/2.1/maptile/newest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /maptile/newest/normal.day/9/255/170/256/png8:
    get:
      summary: Toll Zone Map
      description: |-
        *Request a street map tile highlighting congestion and environmental toll zones*

        To highlight such toll zones, add the `congestion` parameter to the request URL.



        * **congestion**  `null`
         \- Flag to indicate if congestion zones are to be shown on the map.

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: MaptileNewestNormalDay9255170256Png8Get
      x-api-path-slug: maptilenewestnormal-day9255170256png8-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: congestion
      responses:
        200:
          description: OK
      tags:
      - Toll
      - Zone
      - Map
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