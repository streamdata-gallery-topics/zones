{
  "info": {
    "name": "CloudFlare A list of available Custom Pages the zone can use",
    "_postman_id": "5f36dca3-3080-4404-804d-c7a1db3e2027",
    "description": "A list of available Custom Pages the zone can use",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "ef014921-929b-4ab8-b52e-423398328e0e",
          "name": "cloudflare-custom-pages-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_pages",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of available Custom Pages the zone can use"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "308ff401-23a1-4d84-b1ef-a967972e8b25"
            }
          ]
        }
      ]
    }
  ]
}