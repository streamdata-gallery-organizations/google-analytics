{
  "info": {
    "name": "Google Analytics Upload Data",
    "_postman_id": "9c83ffb5-97e9-41bf-af50-15c92e055c56",
    "description": "Upload data for a custom data source.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "data",
      "item": [
        {
          "id": "1cfd8eec-3dab-4765-ba19-47947ac9d637",
          "name": "analytics.management.uploads.uploadData",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "analytics",
                "v3",
                "management/accounts/:accountId/webproperties/:webPropertyId/customDataSources/:customDataSourceId/uploads"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "customDataSourceId",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload data for a custom data source"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37b846ae-524e-41ed-baf2-6cd7363840ca"
            }
          ]
        }
      ]
    }
  ]
}