{
  "info": {
    "name": "Google Analytics Get Custom Data",
    "_postman_id": "3d53d563-1de1-4cce-b3a4-ceb7a8bac9f2",
    "description": "List custom data sources to which the user has access.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "custom data",
      "item": [
        {
          "id": "92c71aee-8169-46c9-9c0d-24e4957045d4",
          "name": "analytics.management.customDataSources.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "analytics",
                "v3",
                "management/accounts/:accountId/webproperties/:webPropertyId/customDataSources"
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
                },
                {
                  "id": "webPropertyId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List custom data sources to which the user has access"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11ad62ab-d9a6-4db2-8705-ffcef44f3ea2"
            }
          ]
        }
      ]
    }
  ]
}