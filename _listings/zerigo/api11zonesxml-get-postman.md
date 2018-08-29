{
  "info": {
    "name": "Zerigo List all zones",
    "_postman_id": "8e6928cd-d455-418c-9f9b-bdf9d19ab8b6",
    "description": "There are two optional parameters: page=# and per_page=#. page defaults to 1 (and starts at 1, not 0). per_page defaults to 100 but should be specified exactly if a change of the default value will cause your application to fail. The maximum value for per_page is 1000.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "756a0281-8fa4-444d-8fb4-94a62f51f05a",
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
              "id": "37931ce1-cef9-491e-ac4a-9228edf36bd3"
            }
          ]
        }
      ]
    }
  ]
}