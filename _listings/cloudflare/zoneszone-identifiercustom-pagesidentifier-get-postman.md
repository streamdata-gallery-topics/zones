{
  "info": {
    "name": "CloudFlare Details about a specific Custom page details",
    "_postman_id": "3d5253b1-a8a9-492a-997a-2c7614e71515",
    "description": "Details about a specific Custom page details",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "528939a8-7ac1-4af1-862c-790deeb82da4",
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
              "id": "6f22abfd-35ec-46d6-a0bb-22f870af2bd1"
            }
          ]
        },
        {
          "id": "bf98a045-2c0e-417d-878b-26d7ad396158",
          "name": "cloudflare-custom-pages-for-a-zone-api1",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_pages/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about a specific Custom page details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a207366-b6f6-464f-8161-04ce854e3167"
            }
          ]
        }
      ]
    }
  ]
}