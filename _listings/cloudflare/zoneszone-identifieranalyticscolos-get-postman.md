{
  "info": {
    "name": "CloudFlare This view provides a breakdown of analytics data by datacenter",
    "_postman_id": "b4561d84-c725-45ef-a630-bfcda1a06729",
    "description": "This view provides a breakdown of analytics data by datacenter",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "081daa7a-77f1-4d85-ab19-91712ce83502",
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
              "id": "99773612-7ac6-4c3f-bcb4-1693ffad31ef"
            }
          ]
        }
      ]
    }
  ]
}