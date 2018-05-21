{
  "info": {
    "name": "CloudFlare Remove ALL files from CloudFlare&#39;s cache",
    "_postman_id": "7b7ce6cd-6f00-47ea-b763-ce145b87b98a",
    "description": "Remove ALL files from CloudFlare&#39;s cache",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "74b70525-eb4d-4c06-9816-ad7b2df3e082",
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
              "id": "15eb0e2f-d10c-464c-9d58-04e7663a36dc"
            }
          ]
        },
        {
          "id": "a383970d-4406-4eb2-9dba-bacba28f0585",
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
              "id": "6e0fd5ce-c700-45cc-9d92-991592a0cd27"
            }
          ]
        },
        {
          "id": "26166265-f4c4-44d0-a2ed-fcbdd6092635",
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
              "id": "bdac396c-673f-4b03-ab0a-2260d6c4e754"
            }
          ]
        },
        {
          "id": "58ece1e2-9a4c-46ca-9a76-7810b5eb3b72",
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
              "id": "6408721d-c853-48f4-98c0-b1f8c387cc99"
            }
          ]
        },
        {
          "id": "a0233282-ffdd-4350-af2c-d60ded632c94",
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
              "id": "bef26b20-2e3a-4dd4-affd-b73e87334e77"
            }
          ]
        },
        {
          "id": "30b5becc-2d64-4fa8-9422-a82718ea3824",
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
              "id": "11f988e9-3530-424f-9b5a-83e6ad91549e"
            }
          ]
        },
        {
          "id": "658a6714-7eda-42a9-ab30-c36daa12a7d4",
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
              "id": "cbb977b9-e141-4e0c-98fc-94f1281cf1a8"
            }
          ]
        },
        {
          "id": "fc492571-52fb-4f81-b854-c69135bea6c6",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Zone details permission needed: #zone:readntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c84500a-ebd5-49a4-a8b7-40a8ed2d6571"
            }
          ]
        },
        {
          "id": "e553841a-94f9-4d19-a313-79361b010fab",
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
              "id": "1d4e2e33-1ac8-42ec-abb2-a14e6ae016f3"
            }
          ]
        },
        {
          "id": "7c06990a-84f3-441d-b258-508a3de03f4b",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:identifier?paused=%7B%7D&plan=%7B%7D&vanity_name_servers=%7B%7D",
            "method": "PATCH",
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
            "description": "Only one zone property can be changed at a time"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cf29a4d-233e-4d09-b1d3-5e3207e6d0b4"
            }
          ]
        },
        {
          "id": "577421b4-98e3-4446-8b38-cc1a8185de11",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:identifier/activation_check",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Initiate another zone activation check permission needed: #zone:editntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c90fd46-904c-4526-8f02-99bc26fca75e"
            }
          ]
        },
        {
          "id": "10723d30-07a4-4022-837a-51f35d60f93e",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:identifier/purge_cache?files=%7B%7D&purge_everything=%7B%7D&tags=%7B%7D",
            "method": "DELETE",
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
            "description": "Remove ALL files from CloudFlare&#39;s cache"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "088a21b8-b938-472b-a40a-a87211a3928d"
            }
          ]
        }
      ]
    }
  ]
}