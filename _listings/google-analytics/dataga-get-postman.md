{
  "info": {
    "name": "Google Analytics Return Analytics Data",
    "_postman_id": "52efafae-a7ec-49b3-8134-ddde2f4e97ea",
    "description": "Returns Analytics data for a view (profile).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "analytic data",
      "item": [
        {
          "id": "41e3f6bb-bb40-4911-9262-699770c32c4d",
          "name": "analytics.data.ga.get",
          "request": {
            "url": "http://www.googleapis.com/analytics/v3/data/ga?dimensions=%7B%7D&end-date=%7B%7D&filters=%7B%7D&ids=%7B%7D&include-empty-rows=%7B%7D&max-results=%7B%7D&metrics=%7B%7D&output=%7B%7D&samplingLevel=%7B%7D&segment=%7B%7D&sort=%7B%7D&start-date=%7B%7D&start-index=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns Analytics data for a view (profile)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3aef78a-47aa-4524-b06c-be676b190373"
            }
          ]
        }
      ]
    }
  ]
}