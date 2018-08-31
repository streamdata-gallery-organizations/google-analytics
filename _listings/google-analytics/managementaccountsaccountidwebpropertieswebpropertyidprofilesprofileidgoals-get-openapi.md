---
swagger: "2.0"
x-collection-name: Google Analytics
x-complete: 0
info:
  title: Google Analytics Get Goals
  description: Lists goals to which the user has access.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /analytics/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /data/ga:
    get:
      summary: Return Analytics Data
      description: Returns Analytics data for a view (profile).
      operationId: analytics.data.ga.get
      x-api-path-slug: dataga-get
      parameters:
      - in: query
        name: dimensions
        description: A comma-separated list of Analytics dimensions
      - in: query
        name: end-date
        description: End date for fetching Analytics data
      - in: query
        name: filters
        description: A comma-separated list of dimension or metric filters to be applied
          to Analytics data
      - in: query
        name: ids
        description: Unique table ID for retrieving Analytics data
      - in: query
        name: include-empty-rows
        description: The response will include empty rows if this parameter is set
          to true, the default is true
      - in: query
        name: max-results
        description: The maximum number of entries to include in this feed
      - in: query
        name: metrics
        description: A comma-separated list of Analytics metrics
      - in: query
        name: output
        description: The selected format for the response
      - in: query
        name: samplingLevel
        description: The desired sampling level
      - in: query
        name: segment
        description: An Analytics segment to be applied to data
      - in: query
        name: sort
        description: A comma-separated list of dimensions or metrics that determine
          the sort order for Analytics data
      - in: query
        name: start-date
        description: Start date for fetching Analytics data
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      responses:
        200:
          description: OK
      tags:
      - Analytic Data
  /data/mcf:
    get:
      summary: Returns Analytics Multi-Channel Funnels Data
      description: Returns Analytics Multi-Channel Funnels data for a view (profile).
      operationId: analytics.data.mcf.get
      x-api-path-slug: datamcf-get
      parameters:
      - in: query
        name: dimensions
        description: A comma-separated list of Multi-Channel Funnels dimensions
      - in: query
        name: end-date
        description: End date for fetching Analytics data
      - in: query
        name: filters
        description: A comma-separated list of dimension or metric filters to be applied
          to the Analytics data
      - in: query
        name: ids
        description: Unique table ID for retrieving Analytics data
      - in: query
        name: max-results
        description: The maximum number of entries to include in this feed
      - in: query
        name: metrics
        description: A comma-separated list of Multi-Channel Funnels metrics
      - in: query
        name: samplingLevel
        description: The desired sampling level
      - in: query
        name: sort
        description: A comma-separated list of dimensions or metrics that determine
          the sort order for the Analytics data
      - in: query
        name: start-date
        description: Start date for fetching Analytics data
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      responses:
        200:
          description: OK
      tags:
      - Analytic Data
  /data/realtime:
    get:
      summary: Return Real Time Data
      description: Returns real time data for a view (profile).
      operationId: analytics.data.realtime.get
      x-api-path-slug: datarealtime-get
      parameters:
      - in: query
        name: dimensions
        description: A comma-separated list of real time dimensions
      - in: query
        name: filters
        description: A comma-separated list of dimension or metric filters to be applied
          to real time data
      - in: query
        name: ids
        description: Unique table ID for retrieving real time data
      - in: query
        name: max-results
        description: The maximum number of entries to include in this feed
      - in: query
        name: metrics
        description: A comma-separated list of real time metrics
      - in: query
        name: sort
        description: A comma-separated list of dimensions or metrics that determine
          the sort order for real time data
      responses:
        200:
          description: OK
      tags:
      - Real Time Data
  /management/accountSummaries:
    get:
      summary: Get Account Summary
      description: Lists account summaries (lightweight tree comprised of accounts/properties/profiles)
        to which the user has access.
      operationId: analytics.management.accountSummaries.list
      x-api-path-slug: managementaccountsummaries-get
      parameters:
      - in: query
        name: max-results
        description: The maximum number of account summaries to include in this response,
          where the largest acceptable value is 1000
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      responses:
        200:
          description: OK
      tags:
      - Account
  /management/accounts:
    get:
      summary: Get Accounts
      description: Lists all accounts to which the user has access.
      operationId: analytics.management.accounts.list
      x-api-path-slug: managementaccounts-get
      parameters:
      - in: query
        name: max-results
        description: The maximum number of accounts to include in this response
      - in: query
        name: start-index
        description: An index of the first account to retrieve
      responses:
        200:
          description: OK
      tags:
      - Account
  /management/accounts/{accountId}/entityUserLinks:
    get:
      summary: Get users
      description: Lists account-user links for a given account.
      operationId: analytics.management.accountUserLinks.list
      x-api-path-slug: managementaccountsaccountidentityuserlinks-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve the user links for
      - in: query
        name: max-results
        description: The maximum number of account-user links to include in this response
      - in: query
        name: start-index
        description: An index of the first account-user link to retrieve
      responses:
        200:
          description: OK
      tags:
      - User
    post:
      summary: Add New Users
      description: Adds a new user to the given account.
      operationId: analytics.management.accountUserLinks.insert
      x-api-path-slug: managementaccountsaccountidentityuserlinks-post
      parameters:
      - in: path
        name: accountId
        description: Account ID to create the user link for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User
  /management/accounts/{accountId}/entityUserLinks/{linkId}:
    delete:
      summary: Remove User
      description: Removes a user from the given account.
      operationId: analytics.management.accountUserLinks.delete
      x-api-path-slug: managementaccountsaccountidentityuserlinkslinkid-delete
      parameters:
      - in: path
        name: accountId
        description: Account ID to delete the user link for
      - in: path
        name: linkId
        description: Link ID to delete the user link for
      responses:
        200:
          description: OK
      tags:
      - User
    put:
      summary: Update Permissions
      description: Updates permissions for an existing user on the given account.
      operationId: analytics.management.accountUserLinks.update
      x-api-path-slug: managementaccountsaccountidentityuserlinkslinkid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID to update the account-user link for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: linkId
        description: Link ID to update the account-user link for
      responses:
        200:
          description: OK
      tags:
      - Permission
  /management/accounts/{accountId}/filters:
    get:
      summary: Get Filters
      description: Lists all filters for an account
      operationId: analytics.management.filters.list
      x-api-path-slug: managementaccountsaccountidfilters-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve filters for
      - in: query
        name: max-results
        description: The maximum number of filters to include in this response
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      responses:
        200:
          description: OK
      tags:
      - Filter
    post:
      summary: Create Filter
      description: Create a new filter.
      operationId: analytics.management.filters.insert
      x-api-path-slug: managementaccountsaccountidfilters-post
      parameters:
      - in: path
        name: accountId
        description: Account ID to create filter for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Filter
  /management/accounts/{accountId}/filters/{filterId}:
    delete:
      summary: Delete Filter
      description: Delete a filter.
      operationId: analytics.management.filters.delete
      x-api-path-slug: managementaccountsaccountidfiltersfilterid-delete
      parameters:
      - in: path
        name: accountId
        description: Account ID to delete the filter for
      - in: path
        name: filterId
        description: ID of the filter to be deleted
      responses:
        200:
          description: OK
      tags:
      - Filter
    get:
      summary: Get Filter
      description: Returns a filters to which the user has access.
      operationId: analytics.management.filters.get
      x-api-path-slug: managementaccountsaccountidfiltersfilterid-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve filters for
      - in: path
        name: filterId
        description: Filter ID to retrieve filters for
      responses:
        200:
          description: OK
      tags:
      - Filter
    patch:
      summary: Update Filter
      description: Updates an existing filter. This method supports patch semantics.
      operationId: analytics.management.filters.patch
      x-api-path-slug: managementaccountsaccountidfiltersfilterid-patch
      parameters:
      - in: path
        name: accountId
        description: Account ID to which the filter belongs
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: filterId
        description: ID of the filter to be updated
      responses:
        200:
          description: OK
      tags:
      - Filter
    put:
      summary: Update Filter
      description: Updates an existing filter.
      operationId: analytics.management.filters.update
      x-api-path-slug: managementaccountsaccountidfiltersfilterid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID to which the filter belongs
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: filterId
        description: ID of the filter to be updated
      responses:
        200:
          description: OK
      tags:
      - Filter
  /management/accounts/{accountId}/webproperties:
    get:
      summary: Get Web Properties
      description: Lists web properties to which the user has access.
      operationId: analytics.management.webproperties.list
      x-api-path-slug: managementaccountsaccountidwebproperties-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve web properties for
      - in: query
        name: max-results
        description: The maximum number of web properties to include in this response
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      responses:
        200:
          description: OK
      tags:
      - Web Property
    post:
      summary: Create Web Property
      description: Create a new property if the account has fewer than 20 properties.
        Web properties are visible in the Google Analytics interface only if they
        have at least one profile.
      operationId: analytics.management.webproperties.insert
      x-api-path-slug: managementaccountsaccountidwebproperties-post
      parameters:
      - in: path
        name: accountId
        description: Account ID to create the web property for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Web Property
  /management/accounts/{accountId}/webproperties/{webPropertyId}:
    get:
      summary: Get Web Property
      description: Gets a web property to which the user has access.
      operationId: analytics.management.webproperties.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyid-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve the web property for
      - in: path
        name: webPropertyId
        description: ID to retrieve the web property for
      responses:
        200:
          description: OK
      tags:
      - Web Property
    patch:
      summary: Update Web Property
      description: Updates an existing web property. This method supports patch semantics.
      operationId: analytics.management.webproperties.patch
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyid-patch
      parameters:
      - in: path
        name: accountId
        description: Account ID to which the web property belongs
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: webPropertyId
        description: Web property ID
      responses:
        200:
          description: OK
      tags:
      - Web Property
    put:
      summary: Update Web Property
      description: Updates an existing web property.
      operationId: analytics.management.webproperties.update
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID to which the web property belongs
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: webPropertyId
        description: Web property ID
      responses:
        200:
          description: OK
      tags:
      - Web Property
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customDataSources:
    get:
      summary: Get Custom Data
      description: List custom data sources to which the user has access.
      operationId: analytics.management.customDataSources.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdatasources-get
      parameters:
      - in: path
        name: accountId
        description: Account Id for the custom data sources to retrieve
      - in: query
        name: max-results
        description: The maximum number of custom data sources to include in this
          response
      - in: query
        name: start-index
        description: A 1-based index of the first custom data source to retrieve
      - in: path
        name: webPropertyId
        description: Web property Id for the custom data sources to retrieve
      responses:
        200:
          description: OK
      tags:
      - Custom Data
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customDataSources/{customDataSourceId}/deleteUploadData:
    post:
      summary: Delete Data
      description: Delete data associated with a previous upload.
      operationId: analytics.management.uploads.deleteUploadData
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdatasourcescustomdatasourceiddeleteuploaddata-post
      parameters:
      - in: path
        name: accountId
        description: Account Id for the uploads to be deleted
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customDataSourceId
        description: Custom data source Id for the uploads to be deleted
      - in: path
        name: webPropertyId
        description: Web property Id for the uploads to be deleted
      responses:
        200:
          description: OK
      tags:
      - Data
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customDataSources/{customDataSourceId}/uploads:
    get:
      summary: List Uploads
      description: List uploads to which the user has access.
      operationId: analytics.management.uploads.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdatasourcescustomdatasourceiduploads-get
      parameters:
      - in: path
        name: accountId
        description: Account Id for the uploads to retrieve
      - in: path
        name: customDataSourceId
        description: Custom data source Id for uploads to retrieve
      - in: query
        name: max-results
        description: The maximum number of uploads to include in this response
      - in: query
        name: start-index
        description: A 1-based index of the first upload to retrieve
      - in: path
        name: webPropertyId
        description: Web property Id for the uploads to retrieve
      responses:
        200:
          description: OK
      tags:
      - Upload
    post:
      summary: Upload Data
      description: Upload data for a custom data source.
      operationId: analytics.management.uploads.uploadData
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdatasourcescustomdatasourceiduploads-post
      parameters:
      - in: path
        name: accountId
        description: Account Id associated with the upload
      - in: path
        name: customDataSourceId
        description: Custom data source Id to which the data being uploaded belongs
      - in: path
        name: webPropertyId
        description: Web property UA-string associated with the upload
      responses:
        200:
          description: OK
      tags:
      - Data
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customDataSources/{customDataSourceId}/uploads/{uploadId}:
    get:
      summary: Get UPloads
      description: List uploads to which the user has access.
      operationId: analytics.management.uploads.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdatasourcescustomdatasourceiduploadsuploadid-get
      parameters:
      - in: path
        name: accountId
        description: Account Id for the upload to retrieve
      - in: path
        name: customDataSourceId
        description: Custom data source Id for upload to retrieve
      - in: path
        name: uploadId
        description: Upload Id to retrieve
      - in: path
        name: webPropertyId
        description: Web property Id for the upload to retrieve
      responses:
        200:
          description: OK
      tags:
      - Upload
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customDimensions:
    get:
      summary: Get Custom Dimensions
      description: Lists custom dimensions to which the user has access.
      operationId: analytics.management.customDimensions.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdimensions-get
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom dimensions to retrieve
      - in: query
        name: max-results
        description: The maximum number of custom dimensions to include in this response
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimensions to retrieve
      responses:
        200:
          description: OK
      tags:
      - Dimension
    post:
      summary: Create Custom Dimension
      description: Create a new custom dimension.
      operationId: analytics.management.customDimensions.insert
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdimensions-post
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom dimension to create
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimension to create
      responses:
        200:
          description: OK
      tags:
      - Dimension
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customDimensions/{customDimensionId}:
    get:
      summary: Get Custom Dimension
      description: Get a custom dimension to which the user has access.
      operationId: analytics.management.customDimensions.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdimensionscustomdimensionid-get
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom dimension to retrieve
      - in: path
        name: customDimensionId
        description: The ID of the custom dimension to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimension to retrieve
      responses:
        200:
          description: OK
      tags:
      - Dimension
    patch:
      summary: Update Custom Dimensions
      description: Updates an existing custom dimension. This method supports patch
        semantics.
      operationId: analytics.management.customDimensions.patch
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdimensionscustomdimensionid-patch
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom dimension to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customDimensionId
        description: Custom dimension ID for the custom dimension to update
      - in: query
        name: ignoreCustomDataSourceLinks
        description: Force the update and ignore any warnings related to the custom
          dimension being linked to a custom data source / data set
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimension to update
      responses:
        200:
          description: OK
      tags:
      - Dimension
    put:
      summary: Update Custom Dimensions
      description: Updates an existing custom dimension.
      operationId: analytics.management.customDimensions.update
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdimensionscustomdimensionid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom dimension to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customDimensionId
        description: Custom dimension ID for the custom dimension to update
      - in: query
        name: ignoreCustomDataSourceLinks
        description: Force the update and ignore any warnings related to the custom
          dimension being linked to a custom data source / data set
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimension to update
      responses:
        200:
          description: OK
      tags:
      - Dimension
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customMetrics:
    get:
      summary: Get Custom Metrics
      description: Lists custom metrics to which the user has access.
      operationId: analytics.management.customMetrics.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustommetrics-get
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom metrics to retrieve
      - in: query
        name: max-results
        description: The maximum number of custom metrics to include in this response
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID for the custom metrics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Metric
    post:
      summary: Create Custom Metric
      description: Create a new custom metric.
      operationId: analytics.management.customMetrics.insert
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustommetrics-post
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom metric to create
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimension to create
      responses:
        200:
          description: OK
      tags:
      - Metric
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customMetrics/{customMetricId}:
    get:
      summary: Get Custom Metric
      description: Get a custom metric to which the user has access.
      operationId: analytics.management.customMetrics.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustommetricscustommetricid-get
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom metric to retrieve
      - in: path
        name: customMetricId
        description: The ID of the custom metric to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID for the custom metric to retrieve
      responses:
        200:
          description: OK
      tags:
      - Metric
    patch:
      summary: Update Custom Metric
      description: Updates an existing custom metric. This method supports patch semantics.
      operationId: analytics.management.customMetrics.patch
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustommetricscustommetricid-patch
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom metric to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customMetricId
        description: Custom metric ID for the custom metric to update
      - in: query
        name: ignoreCustomDataSourceLinks
        description: Force the update and ignore any warnings related to the custom
          metric being linked to a custom data source / data set
      - in: path
        name: webPropertyId
        description: Web property ID for the custom metric to update
      responses:
        200:
          description: OK
      tags:
      - Metric
    put:
      summary: Update Custom Metric
      description: Updates an existing custom metric.
      operationId: analytics.management.customMetrics.update
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustommetricscustommetricid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom metric to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customMetricId
        description: Custom metric ID for the custom metric to update
      - in: query
        name: ignoreCustomDataSourceLinks
        description: Force the update and ignore any warnings related to the custom
          metric being linked to a custom data source / data set
      - in: path
        name: webPropertyId
        description: Web property ID for the custom metric to update
      responses:
        200:
          description: OK
      tags:
      - Metric
  /management/accounts/{accountId}/webproperties/{webPropertyId}/entityAdWordsLinks:
    get:
      summary: List AdWords
      description: Lists webProperty-AdWords links for a given web property.
      operationId: analytics.management.webPropertyAdWordsLinks.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinks-get
      parameters:
      - in: path
        name: accountId
        description: ID of the account which the given web property belongs to
      - in: query
        name: max-results
        description: The maximum number of webProperty-AdWords links to include in
          this response
      - in: query
        name: start-index
        description: An index of the first webProperty-AdWords link to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID to retrieve the AdWords links for
      responses:
        200:
          description: OK
      tags:
      - AdWord
    post:
      summary: Create AdWord
      description: Creates a webProperty-AdWords link.
      operationId: analytics.management.webPropertyAdWordsLinks.insert
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinks-post
      parameters:
      - in: path
        name: accountId
        description: ID of the Google Analytics account to create the link for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: webPropertyId
        description: Web property ID to create the link for
      responses:
        200:
          description: OK
      tags:
      - AdWord
  /management/accounts/{accountId}/webproperties/{webPropertyId}/entityAdWordsLinks/{webPropertyAdWordsLinkId}:
    delete:
      summary: Delete AdWord
      description: Deletes a web property-AdWords link.
      operationId: analytics.management.webPropertyAdWordsLinks.delete
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinkswebpropertyadwordslinkid-delete
      parameters:
      - in: path
        name: accountId
        description: ID of the account which the given web property belongs to
      - in: path
        name: webPropertyAdWordsLinkId
        description: Web property AdWords link ID
      - in: path
        name: webPropertyId
        description: Web property ID to delete the AdWords link for
      responses:
        200:
          description: OK
      tags:
      - AdWord
    get:
      summary: Get AdWord
      description: Returns a web property-AdWords link to which the user has access.
      operationId: analytics.management.webPropertyAdWordsLinks.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinkswebpropertyadwordslinkid-get
      parameters:
      - in: path
        name: accountId
        description: ID of the account which the given web property belongs to
      - in: path
        name: webPropertyAdWordsLinkId
        description: Web property-AdWords link ID
      - in: path
        name: webPropertyId
        description: Web property ID to retrieve the AdWords link for
      responses:
        200:
          description: OK
      tags:
      - AdWord
    patch:
      summary: Update AdWord
      description: Updates an existing webProperty-AdWords link. This method supports
        patch semantics.
      operationId: analytics.management.webPropertyAdWordsLinks.patch
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinkswebpropertyadwordslinkid-patch
      parameters:
      - in: path
        name: accountId
        description: ID of the account which the given web property belongs to
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: webPropertyAdWordsLinkId
        description: Web property-AdWords link ID
      - in: path
        name: webPropertyId
        description: Web property ID to retrieve the AdWords link for
      responses:
        200:
          description: OK
      tags:
      - AdWord
    put:
      summary: Update AdWord
      description: Updates an existing webProperty-AdWords link.
      operationId: analytics.management.webPropertyAdWordsLinks.update
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinkswebpropertyadwordslinkid-put
      parameters:
      - in: path
        name: accountId
        description: ID of the account which the given web property belongs to
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: webPropertyAdWordsLinkId
        description: Web property-AdWords link ID
      - in: path
        name: webPropertyId
        description: Web property ID to retrieve the AdWords link for
      responses:
        200:
          description: OK
      tags:
      - AdWord
  /management/accounts/{accountId}/webproperties/{webPropertyId}/entityUserLinks:
    get:
      summary: Get Users
      description: Lists webProperty-user links for a given web property.
      operationId: analytics.management.webpropertyUserLinks.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidentityuserlinks-get
      parameters:
      - in: path
        name: accountId
        description: Account ID which the given web property belongs to
      - in: query
        name: max-results
        description: The maximum number of webProperty-user Links to include in this
          response
      - in: query
        name: start-index
        description: An index of the first webProperty-user link to retrieve
      - in: path
        name: webPropertyId
        description: Web Property ID for the webProperty-user links to retrieve
      responses:
        200:
          description: OK
      tags:
      - User
    post:
      summary: Add User
      description: Adds a new user to the given web property.
      operationId: analytics.management.webpropertyUserLinks.insert
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidentityuserlinks-post
      parameters:
      - in: path
        name: accountId
        description: Account ID to create the user link for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: webPropertyId
        description: Web Property ID to create the user link for
      responses:
        200:
          description: OK
      tags:
      - User
  /management/accounts/{accountId}/webproperties/{webPropertyId}/entityUserLinks/{linkId}:
    delete:
      summary: Remove User
      description: Removes a user from the given web property.
      operationId: analytics.management.webpropertyUserLinks.delete
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidentityuserlinkslinkid-delete
      parameters:
      - in: path
        name: accountId
        description: Account ID to delete the user link for
      - in: path
        name: linkId
        description: Link ID to delete the user link for
      - in: path
        name: webPropertyId
        description: Web Property ID to delete the user link for
      responses:
        200:
          description: OK
      tags:
      - User
    put:
      summary: Update Permission
      description: Updates permissions for an existing user on the given web property.
      operationId: analytics.management.webpropertyUserLinks.update
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidentityuserlinkslinkid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID to update the account-user link for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: linkId
        description: Link ID to update the account-user link for
      - in: path
        name: webPropertyId
        description: Web property ID to update the account-user link for
      responses:
        200:
          description: OK
      tags:
      - Permission
  /management/accounts/{accountId}/webproperties/{webPropertyId}/profiles:
    get:
      summary: List Views
      description: Lists views (profiles) to which the user has access.
      operationId: analytics.management.profiles.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofiles-get
      parameters:
      - in: path
        name: accountId
        description: Account ID for the view (profiles) to retrieve
      - in: query
        name: max-results
        description: The maximum number of views (profiles) to include in this response
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID for the views (profiles) to retrieve
      responses:
        200:
          description: OK
      tags:
      - View
    post:
      summary: Create View
      description: Create a new view (profile).
      operationId: analytics.management.profiles.insert
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofiles-post
      parameters:
      - in: path
        name: accountId
        description: Account ID to create the view (profile) for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: webPropertyId
        description: Web property ID to create the view (profile) for
      responses:
        200:
          description: OK
      tags:
      - View
  /management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}:
    delete:
      summary: Delete View
      description: Deletes a view (profile).
      operationId: analytics.management.profiles.delete
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileid-delete
      parameters:
      - in: path
        name: accountId
        description: Account ID to delete the view (profile) for
      - in: path
        name: profileId
        description: ID of the view (profile) to be deleted
      - in: path
        name: webPropertyId
        description: Web property ID to delete the view (profile) for
      responses:
        200:
          description: OK
      tags:
      - View
    get:
      summary: Get View
      description: Gets a view (profile) to which the user has access.
      operationId: analytics.management.profiles.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileid-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve the view (profile) for
      - in: path
        name: profileId
        description: View (Profile) ID to retrieve the view (profile) for
      - in: path
        name: webPropertyId
        description: Web property ID to retrieve the view (profile) for
      responses:
        200:
          description: OK
      tags:
      - View
    patch:
      summary: Update View
      description: Updates an existing view (profile). This method supports patch
        semantics.
      operationId: analytics.management.profiles.patch
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileid-patch
      parameters:
      - in: path
        name: accountId
        description: Account ID to which the view (profile) belongs
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: ID of the view (profile) to be updated
      - in: path
        name: webPropertyId
        description: Web property ID to which the view (profile) belongs
      responses:
        200:
          description: OK
      tags:
      - View
    put:
      summary: Update View
      description: Updates an existing view (profile).
      operationId: analytics.management.profiles.update
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID to which the view (profile) belongs
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: ID of the view (profile) to be updated
      - in: path
        name: webPropertyId
        description: Web property ID to which the view (profile) belongs
      responses:
        200:
          description: OK
      tags:
      - View
  /management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/entityUserLinks:
    get:
      summary: List Users
      description: Lists profile-user links for a given view (profile).
      operationId: analytics.management.profileUserLinks.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidentityuserlinks-get
      parameters:
      - in: path
        name: accountId
        description: Account ID which the given view (profile) belongs to
      - in: query
        name: max-results
        description: The maximum number of profile-user links to include in this response
      - in: path
        name: profileId
        description: View (Profile) ID to retrieve the profile-user links for
      - in: query
        name: start-index
        description: An index of the first profile-user link to retrieve
      - in: path
        name: webPropertyId
        description: Web Property ID which the given view (profile) belongs to
      responses:
        200:
          description: OK
      tags:
      - User
    post:
      summary: Add User
      description: Adds a new user to the given view (profile).
      operationId: analytics.management.profileUserLinks.insert
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidentityuserlinks-post
      parameters:
      - in: path
        name: accountId
        description: Account ID to create the user link for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: View (Profile) ID to create the user link for
      - in: path
        name: webPropertyId
        description: Web Property ID to create the user link for
      responses:
        200:
          description: OK
      tags:
      - User
  /management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/entityUserLinks/{linkId}:
    delete:
      summary: Remove User
      description: Removes a user from the given view (profile).
      operationId: analytics.management.profileUserLinks.delete
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidentityuserlinkslinkid-delete
      parameters:
      - in: path
        name: accountId
        description: Account ID to delete the user link for
      - in: path
        name: linkId
        description: Link ID to delete the user link for
      - in: path
        name: profileId
        description: View (Profile) ID to delete the user link for
      - in: path
        name: webPropertyId
        description: Web Property ID to delete the user link for
      responses:
        200:
          description: OK
      tags:
      - User
    put:
      summary: Update Permissions
      description: Updates permissions for an existing user on the given view (profile).
      operationId: analytics.management.profileUserLinks.update
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidentityuserlinkslinkid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID to update the user link for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: linkId
        description: Link ID to update the user link for
      - in: path
        name: profileId
        description: View (Profile ID) to update the user link for
      - in: path
        name: webPropertyId
        description: Web Property ID to update the user link for
      responses:
        200:
          description: OK
      tags:
      - Permission
  /management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/experiments:
    get:
      summary: List Experiments
      description: Lists experiments to which the user has access.
      operationId: analytics.management.experiments.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperiments-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve experiments for
      - in: query
        name: max-results
        description: The maximum number of experiments to include in this response
      - in: path
        name: profileId
        description: View (Profile) ID to retrieve experiments for
      - in: query
        name: start-index
        description: An index of the first experiment to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID to retrieve experiments for
      responses:
        200:
          description: OK
      tags:
      - Experiment
    post:
      summary: Create Experiment
      description: Create a new experiment.
      operationId: analytics.management.experiments.insert
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperiments-post
      parameters:
      - in: path
        name: accountId
        description: Account ID to create the experiment for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: View (Profile) ID to create the experiment for
      - in: path
        name: webPropertyId
        description: Web property ID to create the experiment for
      responses:
        200:
          description: OK
      tags:
      - Experiment
  /management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/experiments/{experimentId}:
    delete:
      summary: Delete Experiment
      description: Delete an experiment.
      operationId: analytics.management.experiments.delete
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperimentsexperimentid-delete
      parameters:
      - in: path
        name: accountId
        description: Account ID to which the experiment belongs
      - in: path
        name: experimentId
        description: ID of the experiment to delete
      - in: path
        name: profileId
        description: View (Profile) ID to which the experiment belongs
      - in: path
        name: webPropertyId
        description: Web property ID to which the experiment belongs
      responses:
        200:
          description: OK
      tags:
      - Experiment
    get:
      summary: Get Experiment
      description: Returns an experiment to which the user has access.
      operationId: analytics.management.experiments.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperimentsexperimentid-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve the experiment for
      - in: path
        name: experimentId
        description: Experiment ID to retrieve the experiment for
      - in: path
        name: profileId
        description: View (Profile) ID to retrieve the experiment for
      - in: path
        name: webPropertyId
        description: Web property ID to retrieve the experiment for
      responses:
        200:
          description: OK
      tags:
      - Experiment
    patch:
      summary: Update Experiment
      description: Update an existing experiment. This method supports patch semantics.
      operationId: analytics.management.experiments.patch
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperimentsexperimentid-patch
      parameters:
      - in: path
        name: accountId
        description: Account ID of the experiment to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: experimentId
        description: Experiment ID of the experiment to update
      - in: path
        name: profileId
        description: View (Profile) ID of the experiment to update
      - in: path
        name: webPropertyId
        description: Web property ID of the experiment to update
      responses:
        200:
          description: OK
      tags:
      - Experiment
    put:
      summary: Update Experiment
      description: Update an existing experiment.
      operationId: analytics.management.experiments.update
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperimentsexperimentid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID of the experiment to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: experimentId
        description: Experiment ID of the experiment to update
      - in: path
        name: profileId
        description: View (Profile) ID of the experiment to update
      - in: path
        name: webPropertyId
        description: Web property ID of the experiment to update
      responses:
        200:
          description: OK
      tags:
      - Experiment
  /management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/goals:
    get:
      summary: Get Goals
      description: Lists goals to which the user has access.
      operationId: analytics.management.goals.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidgoals-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve goals for
      - in: query
        name: max-results
        description: The maximum number of goals to include in this response
      - in: path
        name: profileId
        description: View (Profile) ID to retrieve goals for
      - in: query
        name: start-index
        description: An index of the first goal to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID to retrieve goals for
      responses:
        200:
          description: OK
      tags:
      - Goal
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---