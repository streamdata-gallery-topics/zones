---
swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 0
info:
  title: AWS Route 53 API List Hosted Zones
  version: 1.0.0
  description: 'To retrieve a list of your public and private hosted zones, send a
    GETrequest to the /2013-04-01/hostedzone resource. The response to this requestincludes
    a HostedZones child element for each hosted zone created by the currentAWS account.Amazon
    Route 53 returns a maximum of 100 items in each response. If you have a lot of
    hostedzones, you can use the maxitems parameter to list them in groups of up to
    100.The response includes four values that help navigate from one group of maxitemshosted
    zones to the next:                  MaxItems is the value specified for the maxitems
    parameterin the request that produced the current response.If the value of IsTruncated
    in the response is true, there are morehosted zones associated with the current
    AWS account.                   NextMarker is the hosted zone ID of the next hosted
    zone that isassociated with the current AWS account. If you want to list more
    hosted zones, makeanother call to ListHostedZones, and specify the value of theNextMarker
    element in the marker parameter. If IsTruncated is false, the NextMarker element
    isomitted from the response.If you''re making the second or subsequent call to
    ListHostedZones, theMarker element matches the value that you specified in themarker
    parameter in the previous request.'
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/hostedzone&amp;delegationsetid=DelegationSetId?marker=Marker&amp;maxitems=MaxItems:
    get:
      summary: List Hosted Zones
      description: 'To retrieve a list of your public and private hosted zones, send
        a GETrequest to the /2013-04-01/hostedzone resource. The response to this
        requestincludes a HostedZones child element for each hosted zone created by
        the currentAWS account.Amazon Route 53 returns a maximum of 100 items in each
        response. If you have a lot of hostedzones, you can use the maxitems parameter
        to list them in groups of up to 100.The response includes four values that
        help navigate from one group of maxitemshosted zones to the next:                  MaxItems
        is the value specified for the maxitems parameterin the request that produced
        the current response.If the value of IsTruncated in the response is true,
        there are morehosted zones associated with the current AWS account.                   NextMarker
        is the hosted zone ID of the next hosted zone that isassociated with the current
        AWS account. If you want to list more hosted zones, makeanother call to ListHostedZones,
        and specify the value of theNextMarker element in the marker parameter. If
        IsTruncated is false, the NextMarker element isomitted from the response.If
        you''re making the second or subsequent call to ListHostedZones, theMarker
        element matches the value that you specified in themarker parameter in the
        previous request.'
      operationId: listhostedzones
      x-api-path-slug: 20130401hostedzoneampdelegationsetiddelegationsetidmarkermarkerampmaxitemsmaxitems-get
      parameters:
      - in: path
        name: delegationsetid
        description: If youre using reusable delegation sets and you want to list
          all of the hosted zones that are associated with a reusable delegation set,
          specify the ID of that reusable delegation set
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hosted Zones
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