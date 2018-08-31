{
  "info": {
    "name": "Google Analytics Get Remarketing Audiences",
    "_postman_id": "f1f35c82-c522-466a-b7da-9462afaa73ed",
    "description": "Lists remarketing audiences to which the user has access.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "remarketing audience",
      "item": [
        {
          "id": "43e44ca0-d7f1-4fc8-9f8b-3f659e7c8bd6",
          "name": "analytics.management.remarketingAudience.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "analytics",
                "v3",
                "management/accounts/:accountId/webproperties/:webPropertyId/remarketingAudiences"
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
                },
                {
                  "key": "type",
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
            "description": "Lists remarketing audiences to which the user has access"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84882884-16c1-4a1b-a40f-6debe13ad294"
            }
          ]
        }
      ]
    }
  ]
}