{
  "info": {
    "name": "Google Analytics Get Remarketing Audience",
    "_postman_id": "d8b8fe1e-529a-4b6c-94c4-2c665f379453",
    "description": "Gets a remarketing audience to which the user has access.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "remarketing audience",
      "item": [
        {
          "id": "1a78fc84-10d8-4099-899c-6c627eb11771",
          "name": "analytics.management.remarketingAudience.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "analytics",
                "v3",
                "management/accounts/:accountId/webproperties/:webPropertyId/remarketingAudiences/:remarketingAudienceId"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "remarketingAudienceId",
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
            "description": "Gets a remarketing audience to which the user has access"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "976c71d5-872c-433d-b1e5-61b088ca30d9"
            }
          ]
        }
      ]
    }
  ]
}