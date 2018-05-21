{
  "info": {
    "name": "Zerigo Create a zone",
    "_postman_id": "46545259-532d-4610-8df5-0a128ed03d39",
    "description": "ns1 should be left out unless ns-type is &#8216;sec&#8217;. slave-nameservers should be left out unless ns-type is &#8216;pri&#8217;. See more details under Zones Overview.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "37892c5a-de3d-4cd6-987b-ba0c54e70405",
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
              "id": "76272dc9-4b28-4b41-a052-b10d2fa8070f"
            }
          ]
        },
        {
          "id": "5ba6bc27-d2f8-4724-ae41-0c2b8a061ae9",
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
              "id": "9c64077a-307f-46b5-83c9-9e5e182f9b99"
            }
          ]
        },
        {
          "id": "e013fdd9-dbdf-4540-9449-b506e9908fa2",
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
              "id": "6552120b-7ba1-49d4-aef4-227d9d561fee"
            }
          ]
        },
        {
          "id": "f75bf13b-e49d-4460-9ec5-19387c4d6c68",
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
              "id": "066fb357-e693-4c42-9902-d6a43a06c361"
            }
          ]
        }
      ]
    }
  ]
}