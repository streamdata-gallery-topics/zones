{
  "info": {
    "name": "CloudFlare Delete an existing zone",
    "_postman_id": "8773104a-8aeb-4a2f-9343-143172a9a7bb",
    "description": "Delete an existing zone",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "3378b694-44c3-4440-92d5-02de4d8d7a7a",
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
              "id": "f9cd076e-1b19-4ad2-800b-23a8823b16a2"
            }
          ]
        },
        {
          "id": "715d24dc-0cc3-4008-9cf5-37ae33960ed0",
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
              "id": "566e7a33-59a2-4e62-95c8-e67182d0ef9c"
            }
          ]
        },
        {
          "id": "aa927d23-531c-46a8-ab27-93d9fe46cb34",
          "name": "cloudflare-custom-pages-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_pages/:identifier?state=%7B%7D&url=%7B%7D",
            "method": "PUT",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update Custom page URL"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ac447f4-6f73-4d22-acc1-aae96c853273"
            }
          ]
        },
        {
          "id": "12302525-ea10-4a2a-b3e7-2fa506f7ee06",
          "name": "cloudflare-zone-analytics-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/analytics/colos?continuous=%7B%7D&since=%7B%7D&until=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This view provides a breakdown of analytics data by datacenter"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c13ce61-8b37-4f9c-a3f4-ba3b96a053a7"
            }
          ]
        },
        {
          "id": "29bafc6e-2a71-4aee-ae02-5dd77b8f5ea0",
          "name": "cloudflare-zone-analytics-api1",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/analytics/dashboard?continuous=%7B%7D&since=%7B%7D&until=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The dashboard view provides both totals and timeseries data for the given zone and time period across the entire CloudFlare network"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41cc0b24-878c-466e-8595-7532eff61759"
            }
          ]
        },
        {
          "id": "3e730ccc-e7d9-4967-9af8-0f1bab0d324b",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones?direction=%7B%7D&match=%7B%7D&name=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&status=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List, search, sort, and filter your zones"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0dcba7a-7532-4ffe-b1bf-f44768779cb4"
            }
          ]
        },
        {
          "id": "2964a855-dee9-4110-b3f7-fde69c8d260d",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones?name=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The domain name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c8e4895-91b5-433a-84bd-98a82195ab1b"
            }
          ]
        },
        {
          "id": "850e5ec5-69b9-4b2f-8c28-0feb3d0be7ff",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an existing zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "417769bf-9bcb-48ee-af3d-b363742e8e2f"
            }
          ]
        }
      ]
    }
  ]
}