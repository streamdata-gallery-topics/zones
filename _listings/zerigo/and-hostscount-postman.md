{
  "info": {
    "name": "Zerigo Get a zone",
    "_postman_id": "ee9c4464-04db-4a6e-921d-c0a784190847",
    "description": "This response is similar to Listing All Zones, with the addition of hosts-count and possibly hosts. As long as there are no more than 300 hosts, they will be returned. If there are more, the hosts array will be left out. hosts-count will always be returned.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "77ce0bd5-828c-462d-8147-fa55d501d19c",
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
              "id": "cbf4569a-a86a-41fd-9fef-f67a9fe2736f"
            }
          ]
        }
      ]
    }
  ]
}