swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/shipping_zones.json:
    get:
      summary: Show list of shipping zones
      description: Show list of shipping zones.
      operationId: getAdminShippingZones.json
      x-api-path-slug: adminshipping-zones-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Show
      - List
      - Shipping
      - Zones