{
  "info": {
    "name": "Google Analytics Get users",
    "_postman_id": "1940893f-8fef-4e1b-8fdf-3ceddbca4794",
    "description": "Lists account-user links for a given account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analytic Data",
      "item": [
        {
          "id": "189ad558-7c97-4873-8ffc-4ee345aae5de",
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
              "id": "0ed0d9f0-c944-4a6a-abec-736139bc8e60"
            }
          ]
        },
        {
          "id": "4738ea2f-14e5-4416-96d9-b5f4129e6ba2",
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
              "id": "114932c5-e56d-46cf-880e-13bb1320dda6"
            }
          ]
        }
      ]
    },
    {
      "name": "Real Time Data",
      "item": [
        {
          "id": "f8b2bc08-363b-4f46-8028-61a057e66bec",
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
              "id": "cf19a277-30aa-4f9e-88e6-0509a116228b"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "32224fae-8276-463b-bd04-cbfebf332076",
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
              "id": "d2191751-c064-4773-9a3b-6b98c75c0ff1"
            }
          ]
        },
        {
          "id": "3ede2bdc-e63a-4f68-9b22-de01217a4617",
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
              "id": "b8f2c695-c675-44bd-8ee2-8deed6a11faf"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "0322c7ff-d0b2-4401-a789-0820c7eecac9",
          "name": "analytics.management.accountUserLinks.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "analytics",
                "v3",
                "management/accounts/:accountId/entityUserLinks"
              ],
              "query": [
                {
                  "key": "max-results",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start-index",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists account-user links for a given account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2befca6e-c154-45f4-ba67-2f81bd77ef5e"
            }
          ]
        }
      ]
    }
  ]
}