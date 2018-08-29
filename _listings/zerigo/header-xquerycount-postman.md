{
  "info": {
    "name": "Zerigo Count all zones",
    "_postman_id": "33eca9c4-8f2d-4d48-ae28-e8eef85504ae",
    "description": "This is the total number of zones available. It is the same value as provided in the X-Query-Count header in the Managed DNS &#8594; List all zones API method.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "2c9a339d-517f-4eaa-9036-c7e19872ffe1",
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
              "id": "3d406c3b-0304-4df7-a39b-9c787a5d0d66"
            }
          ]
        }
      ]
    }
  ]
}