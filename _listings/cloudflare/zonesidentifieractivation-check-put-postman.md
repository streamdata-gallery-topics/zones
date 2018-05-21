{
  "info": {
    "name": "CloudFlare Initiate another zone activation check permission needed: #zone:edit",
    "_postman_id": "4108e2e7-bd0e-4c3a-a71a-8b5421ee7c44",
    "description": "Initiate another zone activation check permission needed: #zone:editntt",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "46164389-7277-408a-ae92-71264cc44c48",
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
              "id": "f6c43e21-f65a-4b20-843e-f8fc9a99ea86"
            }
          ]
        },
        {
          "id": "8e17dc89-5102-496e-9d33-f9bc14b87dc6",
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
              "id": "37ac637b-e259-4535-a007-6fc619c35c77"
            }
          ]
        },
        {
          "id": "e2e1cc9b-58d1-4d2f-9474-80e1dce30181",
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
              "id": "1c7ab517-7c25-47e0-971a-ede5eabd1a4c"
            }
          ]
        },
        {
          "id": "58607cdb-63dd-4bc4-b616-c808a7750351",
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
              "id": "fc8245c0-dccb-4080-a0ef-4b8177ab7585"
            }
          ]
        },
        {
          "id": "fe8aece6-8ab1-46d6-b7e3-a9b377fd1286",
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
              "id": "4a4a1d58-e589-47fd-971d-fd173f436644"
            }
          ]
        },
        {
          "id": "907dd756-0617-48f5-af85-57fb396200d2",
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
              "id": "6cb5ca26-9a30-4c6c-94aa-d2bbce74ea8b"
            }
          ]
        },
        {
          "id": "e3e55121-d5ec-4878-99f3-d824adbd8e0a",
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
              "id": "b4792c50-b2d0-4e3a-8ed0-24ab4455fd98"
            }
          ]
        },
        {
          "id": "a160c248-d33d-408a-8090-cb603836f2ae",
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
              "id": "972a4816-396e-4e62-8be1-d87bb0cb5d3c"
            }
          ]
        },
        {
          "id": "3c3900ce-ce1d-424f-a89e-a5969ec263ac",
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
              "id": "f6142f6e-473d-4ba0-86db-c1a3cbe1f1f5"
            }
          ]
        },
        {
          "id": "9d91babc-504c-41ad-a325-9f8703e86096",
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
              "id": "d0256071-eff0-4bba-a4a0-ae8f8c8ba441"
            }
          ]
        },
        {
          "id": "a8faa6fb-8884-47e1-9a2f-4c9d7b1975d9",
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
              "id": "29877da1-e3e2-4d7d-80ca-d0f9297c787f"
            }
          ]
        }
      ]
    }
  ]
}