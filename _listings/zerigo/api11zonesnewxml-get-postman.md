{
  "info": {
    "name": "Zerigo Get a blank zone",
    "_postman_id": "31c92357-f0c4-4dc6-8ac7-d4557a45cbed",
    "description": "This response may be useful to obtain a blank zone, suitable for use as a template or retrieving default values for included fields.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "0a536ac7-1079-4afd-98c1-9344d5774d8b",
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
              "id": "02bad82e-c260-40db-be1b-213d9be0d641"
            }
          ]
        },
        {
          "id": "890068cd-9b9b-4231-9bc7-6968ba45c637",
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
              "id": "131b8e9d-b2a8-45b2-a9bf-e3a7314b21c1"
            }
          ]
        },
        {
          "id": "799305aa-c4c6-45b2-afec-3a5b03342cc3",
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
              "id": "d90e5790-69c6-42a4-8542-7112b03c784c"
            }
          ]
        }
      ]
    }
  ]
}