{
  "info": {
    "name": "Google Analytics Get Account Summary",
    "_postman_id": "0fb21f25-33e1-40a1-b98a-ba6c9e10ba84",
    "description": "Lists account summaries (lightweight tree comprised of accounts/properties/profiles) to which the user has access.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analytic Data",
      "item": [
        {
          "id": "4d4625ca-c865-4c33-947b-44551f11707b",
          "name": "analytics.data.ga.get",
          "request": {
            "url": "http://www.googleapis.com/analytics/v3/data/ga?dimensions=%7B%7D&end-date=%7B%7D&filters=%7B%7D&ids=%7B%7D&include-empty-rows=%7B%7D&max-results=%7B%7D&metrics=%7B%7D&output=%7B%7D&samplingLevel=%7B%7D&segment=%7B%7D&sort=%7B%7D&start-date=%7B%7D&start-index=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns Analytics data for a view (profile)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "588c6a02-10a6-429a-b166-8cd1555e7659"
            }
          ]
        },
        {
          "id": "709ac356-4a19-4445-a022-34c56d640a4e",
          "name": "analytics.data.mcf.get",
          "request": {
            "url": "http://www.googleapis.com/analytics/v3/data/mcf?dimensions=%7B%7D&end-date=%7B%7D&filters=%7B%7D&ids=%7B%7D&max-results=%7B%7D&metrics=%7B%7D&samplingLevel=%7B%7D&sort=%7B%7D&start-date=%7B%7D&start-index=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns Analytics Multi-Channel Funnels data for a view (profile)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92436daf-df08-4ec3-b875-ccf9e5c8a3cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Real Time Data",
      "item": [
        {
          "id": "0ed0ea6e-293b-44a0-8652-051b79d776a5",
          "name": "analytics.data.realtime.get",
          "request": {
            "url": "http://www.googleapis.com/analytics/v3/data/realtime?dimensions=%7B%7D&filters=%7B%7D&ids=%7B%7D&max-results=%7B%7D&metrics=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns real time data for a view (profile)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d30cb31-84f6-4152-b19c-72ae5e77de63"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "6070adf8-f26e-479a-a938-9e2b00227be9",
          "name": "analytics.management.accountSummaries.list",
          "request": {
            "url": "http://www.googleapis.com/analytics/v3/management/accountSummaries?max-results=%7B%7D&start-index=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists account summaries (lightweight tree comprised of accounts/properties/profiles) to which the user has access."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bd47891-85df-4740-9ee1-2b0a8d82de26"
            }
          ]
        }
      ]
    }
  ]
}