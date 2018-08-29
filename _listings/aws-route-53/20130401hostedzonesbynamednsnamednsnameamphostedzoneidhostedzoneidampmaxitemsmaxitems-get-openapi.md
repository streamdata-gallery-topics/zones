---
swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 0
info:
  title: AWS Route 53 API List Hosted Zones By Name
  version: 1.0.0
  description: 'Retrieves a list of your hosted zones in lexicographic order. Send
    a GETrequest to the /2013-04-01/hostedzonesbyname resource. The response includes
    aHostedZones child element for each hosted zone created by the current AWSaccount.             ListHostedZonesByName
    sorts hosted zones by name with the labels reversed.For example:                  com.example.www.               Note
    the trailing dot, which can change the sort order in some circumstances.If the
    domain name includes escape characters or Punycode,ListHostedZonesByName alphabetizes
    the domain name using the escaped orPunycoded value, which is the format that
    Amazon Route 53 saves in its database. For example, to createa hosted zone for
    example.com, specify ex\344mple.com for the domain name.ListHostedZonesByName
    alphabetizes it as:                  com.ex\344mple.               The labels
    are reversed and alphabetized using the escaped value. For more informationabout
    valid domain name formats, including internationalized domain names, see DNS Domain
    Name Format in theAmazon Route 53 Developer Guide.Amazon Route 53 returns up to
    100 items in each response. If you have a lot of hosted zones, usethe MaxItems
    parameter to list them in groups of up to 100. The response includesvalues that
    help navigate from one group of MaxItems hosted zones to thenext:The DNSName and
    HostedZoneId elements in the responsecontain the values, if any, specified for
    the dnsname andhostedzoneid parameters in the request that produced the currentresponse.The
    MaxItems element in the response contains the value, if any, thatyou specified
    for the maxitems parameter in the request that produced thecurrent response.If
    the value of IsTruncated in the response is true, there are morehosted zones associated
    with the current AWS account. If IsTruncated is false, this response includes
    the last hosted zonethat is associated with the current account. The NextDNSName
    element andNextHostedZoneId elements are omitted from the response.The NextDNSName
    and NextHostedZoneId elements in theresponse contain the domain name and the hosted
    zone ID of the next hosted zone that isassociated with the current AWS account.
    If you want to list more hosted zones, makeanother call to ListHostedZonesByName,
    and specify the value ofNextDNSName and NextHostedZoneId in the dnsnameand hostedzoneid
    parameters, respectively.'
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
  /2013-04-01/hostedzonesbyname?dnsname=DNSName&amp;hostedzoneid=HostedZoneId&amp;maxitems=MaxItems:
    get:
      summary: List Hosted Zones By Name
      description: 'Retrieves a list of your hosted zones in lexicographic order.
        Send a GETrequest to the /2013-04-01/hostedzonesbyname resource. The response
        includes aHostedZones child element for each hosted zone created by the current
        AWSaccount.             ListHostedZonesByName sorts hosted zones by name with
        the labels reversed.For example:                  com.example.www.               Note
        the trailing dot, which can change the sort order in some circumstances.If
        the domain name includes escape characters or Punycode,ListHostedZonesByName
        alphabetizes the domain name using the escaped orPunycoded value, which is
        the format that Amazon Route 53 saves in its database. For example, to createa
        hosted zone for example.com, specify ex\344mple.com for the domain name.ListHostedZonesByName
        alphabetizes it as:                  com.ex\344mple.               The labels
        are reversed and alphabetized using the escaped value. For more informationabout
        valid domain name formats, including internationalized domain names, see DNS
        Domain Name Format in theAmazon Route 53 Developer Guide.Amazon Route 53 returns
        up to 100 items in each response. If you have a lot of hosted zones, usethe
        MaxItems parameter to list them in groups of up to 100. The response includesvalues
        that help navigate from one group of MaxItems hosted zones to thenext:The
        DNSName and HostedZoneId elements in the responsecontain the values, if any,
        specified for the dnsname andhostedzoneid parameters in the request that produced
        the currentresponse.The MaxItems element in the response contains the value,
        if any, thatyou specified for the maxitems parameter in the request that produced
        thecurrent response.If the value of IsTruncated in the response is true, there
        are morehosted zones associated with the current AWS account. If IsTruncated
        is false, this response includes the last hosted zonethat is associated with
        the current account. The NextDNSName element andNextHostedZoneId elements
        are omitted from the response.The NextDNSName and NextHostedZoneId elements
        in theresponse contain the domain name and the hosted zone ID of the next
        hosted zone that isassociated with the current AWS account. If you want to
        list more hosted zones, makeanother call to ListHostedZonesByName, and specify
        the value ofNextDNSName and NextHostedZoneId in the dnsnameand hostedzoneid
        parameters, respectively.'
      operationId: listhostedzonesbyname
      x-api-path-slug: 20130401hostedzonesbynamednsnamednsnameamphostedzoneidhostedzoneidampmaxitemsmaxitems-get
      parameters:
      - in: path
        name: dnsname
        description: (Optional) For your first request to ListHostedZonesByName, include
          thednsname parameter only if you want to specify the name of the first hosted
          zonein the response
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