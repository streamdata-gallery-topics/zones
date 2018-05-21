{
  "info": {
    "name": "Zerigo Get stats for a zone",
    "_postman_id": "90749f31-b8af-4b78-b2d0-84bc105aedcf",
    "description": "This response returns current traffic statistics about this zone. Queries is measured from the beginning of the current period through the time of the API call. Just like everywhere else in our system, dates are based on UTC.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "3e023c4a-3155-471d-96ea-ce32e5eb3570",
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
              "id": "b7580b16-8cbe-4b89-af23-59e3185936cc"
            }
          ]
        },
        {
          "id": "75d9815e-b43c-42be-b5b8-e2643be68120",
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
              "id": "882e96ca-cf7c-42a0-b086-11a6a2b5d0c1"
            }
          ]
        }
      ]
    }
  ]
}