---
swagger: "2.0"
x-collection-name: AWS Route 53
info:
  title: AWS Route 53 API Delete Hosted Zone
  version: 1.0.0
  description: Deletes a hosted zone. Send a DELETE request to the /Amazon Route 53API
    version/hostedzone/hosted zone ID             resource.ImportantDelete a hosted
    zone only if there are no resource record sets other than the defaultSOA record
    and NS resource record sets. If the hosted zone contains other resource recordsets,
    delete them before deleting the hosted zone. If you try to delete a hosted zone
    thatcontains other resource record sets, Amazon Route 53 denies your request with
    aHostedZoneNotEmpty error. For information about deleting records from yourhosted
    zone, see ChangeResourceRecordSets.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/hostedzone:
    post:
      summary: Create Hosted Zone
      description: Creates a new public hosted zone, used to specify how the Domain
        Name System (DNS)routes traffic on the Internet for a domain, such as example.com,
        and its subdomains. ImportantPublic hosted zones can't be converted to a private
        hosted zone or vice versa.Instead, create a new hosted zone with the same
        name and create new resource recordsets.Send a POST request to the /2013-04-01/hostedzone
        resource. The request body must include a documentwith a CreateHostedZoneRequest
        element. The response returns theCreateHostedZoneResponse element containing
        metadata about the hostedzone.Fore more information about charges for hosted
        zones, see Amazon Route 53 Pricing.Note the following:You can't create a hosted
        zone for a top-level domain (TLD).Amazon Route 53 automatically creates a
        default SOA record and four NS records for the zone.For more information about
        SOA and NS records, see NS and SOA Records that Amazon Route 53 Creates for
        a Hosted Zone in the Amazon Route 53 Developer Guide.If your domain is registered
        with a registrar other than Amazon Route 53, you must update thename servers
        with your registrar to make Amazon Route 53 your DNS service. For more information,
        seeConfiguring Amazon Route 53 as your DNSService in the Amazon Route 53 Developer's
        Guide.After creating a zone, its initial status is PENDING. This means that
        itis not yet available on all DNS servers. The status of the zone changes
        to INSYNCwhen the NS and SOA records are available on all Amazon Route 53
        DNS servers. When trying to create a hosted zone using a reusable delegation
        set, specify anoptional DelegationSetId, and Amazon Route 53 would assign
        those 4 NS records for the zone, instead ofallotting a new one.
      operationId: createhostedzone
      x-api-path-slug: 20130401hostedzone-post
      parameters:
      - in: body
        name: CallerReference
        description: "A unique string that identifies the request and that allows
          failed\t\t\tCreateHostedZone requests to be retried without the risk of
          executing the\t\t\toperation twice"
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: CreateHostedZoneRequest
        description: Root level tag for the CreateHostedZoneRequest parameters
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: Default
        description: None
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: DelegationSetId
        description: "If you want to associate a reusable delegation set with this
          hosted zone, the ID that\t\t\tAmazon Route 53 assigned to the reusable delegation
          set when you created it"
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: HostedZoneConfig
        description: (Optional) A complex type that contains an optional comment about
          your hosted zone
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: Name
        description: The name of the domain
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: Parent
        description: CreatedHostedZoneRequest
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: VPC
        description: The VPC that you want your hosted zone to be associated with
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Hosted Zones
  /2013-04-01/hostedzone/Id:
    delete:
      summary: Delete Hosted Zone
      description: Deletes a hosted zone. Send a DELETE request to the /Amazon Route
        53API version/hostedzone/hosted zone ID             resource.ImportantDelete
        a hosted zone only if there are no resource record sets other than the defaultSOA
        record and NS resource record sets. If the hosted zone contains other resource
        recordsets, delete them before deleting the hosted zone. If you try to delete
        a hosted zone thatcontains other resource record sets, Amazon Route 53 denies
        your request with aHostedZoneNotEmpty error. For information about deleting
        records from yourhosted zone, see ChangeResourceRecordSets.
      operationId: deletehostedzone
      x-api-path-slug: 20130401hostedzoneid-delete
      parameters:
      - in: path
        name: Id
        description: The ID of the hosted zone you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hosted Zones
---