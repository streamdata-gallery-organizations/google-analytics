{
  "info": {
    "name": "Google Analytics Returns Analytics Multi-Channel Funnels Data",
    "_postman_id": "0c15ddbc-50cc-44bd-b533-8d2a49de3398",
    "description": "Returns Analytics Multi-Channel Funnels data for a view (profile).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "analytic data",
      "item": [
        {
          "id": "1b22a1ec-5e25-474e-b8c0-6f1e56941d2f",
          "name": "analytics.data.mcf.get",
          "request": {
            "url": "http://www.googleapis.com/analytics/v3/data/mcf?dimensions=%7B%7D&end-date=%7B%7D&filters=%7B%7D&ids=%7B%7D&max-results=%7B%7D&metrics=%7B%7D&samplingLevel=%7B%7D&sort=%7B%7D&start-date=%7B%7D&start-index=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns Analytics Multi-Channel Funnels data for a view (profile)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8aa08d66-f5c8-4399-a784-12bc5c963a5e"
            }
          ]
        }
      ]
    }
  ]
}