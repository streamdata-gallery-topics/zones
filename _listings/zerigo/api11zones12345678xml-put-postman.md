{
  "info": {
    "name": "Zerigo Update a zone",
    "_postman_id": "80afc980-5bf5-4ea3-b68a-11a807b194a0",
    "description": "ns1 should be left out unless ns-type is &#8216;sec&#8217;. slave-nameservers should be left out unless ns-type is &#8216;pri&#8217;. See more details under Zones Overview.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "391ff22c-8e9f-44a3-a49a-5febddd6a42d",
          "name": "list-all-zones",
          "request": {
            "url": "http://example.com/api/api/1.1/zones.xml",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "There are two optional parameters: page=# and per_page=#. page defaults to 1 (and starts at 1, not 0). per_page defaults to 100 but should be specified exactly if a change of the default value will cause your application to fail. The maximum value for per_page is 1000."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12dcf40c-05ce-4c8e-9b9c-8a96b5ade0c8"
            }
          ]
        },
        {
          "id": "4e050f5a-e07b-4c3f-8c54-9ad98a0e3288",
          "name": "create-a-zone",
          "request": {
            "url": "http://example.com/api/api/1.1/zones.xml",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "ns1 should be left out unless ns-type is &#8216;sec&#8217;. slave-nameservers should be left out unless ns-type is &#8216;pri&#8217;. See more details under Zones Overview."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae2bfa01-c234-47b1-ae7e-97f5992a511e"
            }
          ]
        },
        {
          "id": "4c93b6ff-5aa6-4065-a2b5-5b72368eca8d",
          "name": "get-stats-for-a-zone",
          "request": {
            "url": "http://example.com/api/api/1.1/zones/12345678/stats.xml",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This response returns current traffic statistics about this zone. Queries is measured from the beginning of the current period through the time of the API call. Just like everywhere else in our system, dates are based on UTC."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "709d4ac8-6483-4175-9c0b-9945756124c9"
            }
          ]
        },
        {
          "id": "1eed3125-3887-4154-8a93-58e744597695",
          "name": "get-a-blank-zone",
          "request": {
            "url": "http://example.com/api/api/1.1/zones/new.xml",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This response may be useful to obtain a blank zone, suitable for use as a template or retrieving default values for included fields."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44914eeb-b8b7-4e5d-9a91-057efe9ce4d0"
            }
          ]
        },
        {
          "id": "d0755e22-8115-47f8-82df-205c3c75d928",
          "name": "update-a-zone",
          "request": {
            "url": "http://example.com/api/api/1.1/zones/12345678.xml",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "ns1 should be left out unless ns-type is &#8216;sec&#8217;. slave-nameservers should be left out unless ns-type is &#8216;pri&#8217;. See more details under Zones Overview."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09eef28b-7dbd-4c52-b6ee-2afda7d96c19"
            }
          ]
        }
      ]
    }
  ]
}