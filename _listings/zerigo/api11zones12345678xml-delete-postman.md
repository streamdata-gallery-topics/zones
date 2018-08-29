{
  "info": {
    "name": "Zerigo Delete a zone",
    "_postman_id": "96eb31c9-7440-430d-a985-75a92e748212",
    "description": "Status 200 on success.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "3c9254ec-2f15-4510-be2f-2726f05fd0cf",
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
              "id": "801c7959-f1d0-4cc1-a955-ee960d1da2e2"
            }
          ]
        },
        {
          "id": "c8147fc3-ab31-4cd7-b991-03578a1c6d2b",
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
              "id": "5eacde71-0f33-464e-9f6b-e11a61dfd579"
            }
          ]
        },
        {
          "id": "7b36ef35-e610-4457-83ad-8760728ba176",
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
              "id": "b3b38b95-d199-4e65-a5f3-b93660d6e103"
            }
          ]
        },
        {
          "id": "8f012296-4910-4988-9753-c378b2e9d30d",
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
              "id": "39e1765a-e7b3-4b64-aada-9a8cc75363b5"
            }
          ]
        },
        {
          "id": "59332e8c-7b4a-4d5f-8451-5e8728879213",
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
              "id": "378330c8-1091-46f7-92d6-1a25bd35400f"
            }
          ]
        },
        {
          "id": "c93f49c9-f093-4fe8-bd75-b5ee0b02596d",
          "name": "delete-a-zone",
          "request": {
            "url": "http://example.com/api/api/1.1/zones/12345678.xml",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Status 200 on success."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4e414c4-ed69-4e6c-83b8-2a6d4dd2e9d5"
            }
          ]
        }
      ]
    }
  ]
}