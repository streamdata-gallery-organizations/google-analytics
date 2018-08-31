{
  "info": {
    "name": "Google Analytics Return Real Time Data",
    "_postman_id": "93efb2cd-bbc5-4e95-9b6c-e6bccd7c0761",
    "description": "Returns real time data for a view (profile).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "real time data",
      "item": [
        {
          "id": "26afa835-366a-4bf0-92cb-54d35511689a",
          "name": "analytics.data.realtime.get",
          "request": {
            "url": "http://www.googleapis.com/analytics/v3/data/realtime?dimensions=%7B%7D&filters=%7B%7D&ids=%7B%7D&max-results=%7B%7D&metrics=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns real time data for a view (profile)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8549bbb2-a9f4-43e5-8c2b-98729ea3b2f4"
            }
          ]
        }
      ]
    }
  ]
}