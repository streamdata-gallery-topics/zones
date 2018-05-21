{
  "info": {
    "name": "CloudFlare Zone details permission needed: #zone:read",
    "_postman_id": "0b186b37-806b-444a-affa-a61d86778c0c",
    "description": "Zone details permission needed: #zone:readntt",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "92080439-28ec-4905-a101-f7d63c54ae29",
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
              "id": "46ae88f0-09d1-4b26-bffd-4f422e7b126d"
            }
          ]
        },
        {
          "id": "54ae8cc8-caae-46e8-a836-64ed0adf9c64",
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
              "id": "65de0f72-49cf-4d2e-957e-f6e5d027373a"
            }
          ]
        },
        {
          "id": "47fe177d-ef86-4949-aea6-06dcd6653675",
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
              "id": "7f6791db-7a8b-43e6-8dbc-e069f3779672"
            }
          ]
        },
        {
          "id": "51eb88ae-6d0b-44b5-a08f-34364f5e1790",
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
              "id": "0f3a5c74-6cba-4da7-964e-1486c687e698"
            }
          ]
        },
        {
          "id": "e5161ff5-cc3d-4b94-a07c-caf9fd64ccf9",
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
              "id": "379bee4f-386a-48bc-9856-5e37aa33189d"
            }
          ]
        },
        {
          "id": "9b650b39-40ea-4a58-bf87-382d9794a445",
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
              "id": "3848aaaa-bc88-4a65-bf46-b3719aa68a27"
            }
          ]
        },
        {
          "id": "50d3b1ff-f6d3-41b2-b5d5-1f44c4b3e097",
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
              "id": "21d472d8-2cf2-4a27-bea2-5f57df9d7e46"
            }
          ]
        },
        {
          "id": "88db9675-f61c-4b37-bb15-2115e250014d",
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
              "id": "9f036612-26c3-46a5-b043-fa8b9bb92624"
            }
          ]
        },
        {
          "id": "02b68e12-21b6-484a-9f03-c94af9540bc4",
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
              "id": "a5352717-a307-4e2e-aaa5-a78ba876d81f"
            }
          ]
        }
      ]
    }
  ]
}