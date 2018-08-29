{
  "info": {
    "name": "Eventbrite Get System Timezones",
    "_postman_id": "2df8aad9-abfc-4a74-a3fe-6af4b956c0c0",
    "description": "Returns a paginated response with a key of timezones,\ncontaining a list of timezones.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "System",
      "item": [
        {
          "id": "ba6c7d6e-9531-4190-92be-b42ebde7bd0f",
          "name": "getSystemTimezones",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/system/timezones/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated response with a key of timezones,\ncontaining a list of timezones."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c946cbb-e905-4316-ac89-7a0a24ef44a7"
            }
          ]
        }
      ]
    }
  ]
}