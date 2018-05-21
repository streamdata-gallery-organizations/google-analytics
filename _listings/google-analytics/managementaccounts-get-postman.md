{
  "info": {
    "name": "Google Analytics Get Accounts",
    "_postman_id": "080888b4-e5d9-4edc-93a2-5ac40b01c90a",
    "description": "Lists all accounts to which the user has access.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analytic Data",
      "item": [
        {
          "id": "8a126db3-10ad-43d9-957a-6a7190cf5246",
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
              "id": "5f5ece34-cb11-4da7-916d-ebca84989f1d"
            }
          ]
        },
        {
          "id": "1f2867fc-938b-48d2-b3fe-a0a5b7fb1985",
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
              "id": "1f9cbd66-9348-4414-91f3-514f4218133a"
            }
          ]
        }
      ]
    },
    {
      "name": "Real Time Data",
      "item": [
        {
          "id": "376976e8-b588-4b62-92c9-cb2bb6b8f974",
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
              "id": "ca94ae97-4d73-44bb-aaa2-fb2cb04b6d57"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "63b71bf2-67bc-4676-a017-119effa477bb",
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
              "id": "1121f3f7-6aca-4fc9-b341-f6f2897c9eeb"
            }
          ]
        },
        {
          "id": "2a7d7556-260d-4f52-8ed4-8b93ecc1d950",
          "name": "analytics.management.accounts.list",
          "request": {
            "url": "http://www.googleapis.com/analytics/v3/management/accounts?max-results=%7B%7D&start-index=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all accounts to which the user has access."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f47e929-173e-4b9e-9ae4-19267971c895"
            }
          ]
        }
      ]
    }
  ]
}