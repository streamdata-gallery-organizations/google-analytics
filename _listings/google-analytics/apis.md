---
name: Google Analytics
x-slug: google-analytics
description: Google Analytics gives you the digital analytics tools you need to analyze
  data from all touchpoints in one place, for a deeper understanding of the customer
  experience. You can then share the insights that matter with your whole organization.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Google Analytics
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/apis.md
specificationVersion: "0.14"
apis:
- name: Google Analytics Return Analytics Data
  x-api-slug: google-analytics
  description: Returns Analytics data for a view (profile).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//data/ga
  tags: Analytic Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/dataga-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/dataga-get-openapi.md
- name: Google Analytics Returns Analytics Multi-Channel Funnels Data
  x-api-slug: google-analytics
  description: Returns Analytics Multi-Channel Funnels data for a view (profile).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//data/mcf
  tags: Analytic Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/datamcf-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/datamcf-get-openapi.md
- name: Google Analytics Return Real Time Data
  x-api-slug: google-analytics
  description: Returns real time data for a view (profile).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//data/realtime
  tags: Real Time Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/datarealtime-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/datarealtime-get-openapi.md
- name: Google Analytics Get Account Summary
  x-api-slug: google-analytics
  description: Lists account summaries (lightweight tree comprised of accounts/properties/profiles)
    to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accountSummaries
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsummaries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsummaries-get-openapi.md
- name: Google Analytics Get Accounts
  x-api-slug: google-analytics
  description: Lists all accounts to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccounts-get-openapi.md
- name: Google Analytics Get users
  x-api-slug: google-analytics
  description: Lists account-user links for a given account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/entityUserLinks
  tags: User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidentityuserlinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidentityuserlinks-get-openapi.md
- name: Google Analytics Add New Users
  x-api-slug: google-analytics
  description: Adds a new user to the given account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/entityUserLinks
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidentityuserlinks-post-openapi.md
- name: Google Analytics Remove User
  x-api-slug: google-analytics
  description: Removes a user from the given account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/entityUserLinks/{linkId}
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidentityuserlinkslinkid-delete-openapi.md
- name: Google Analytics Update Permissions
  x-api-slug: google-analytics
  description: Updates permissions for an existing user on the given account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/entityUserLinks/{linkId}
  tags: Permission
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidentityuserlinkslinkid-put-openapi.md
- name: Google Analytics Get Filters
  x-api-slug: google-analytics
  description: Lists all filters for an account
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/filters
  tags: Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidfilters-get-openapi.md
- name: Google Analytics Create Filter
  x-api-slug: google-analytics
  description: Create a new filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/filters
  tags: Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidfilters-post-openapi.md
- name: Google Analytics Delete Filter
  x-api-slug: google-analytics
  description: Delete a filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/filters/{filterId}
  tags: Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidfiltersfilterid-delete-openapi.md
- name: Google Analytics Get Filter
  x-api-slug: google-analytics
  description: Returns a filters to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/filters/{filterId}
  tags: Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidfiltersfilterid-get-openapi.md
- name: Google Analytics Update Filter
  x-api-slug: google-analytics
  description: Updates an existing filter. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/filters/{filterId}
  tags: Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidfiltersfilterid-patch-openapi.md
- name: Google Analytics Update Filter
  x-api-slug: google-analytics
  description: Updates an existing filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/filters/{filterId}
  tags: Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidfiltersfilterid-put-openapi.md
- name: Google Analytics Get Web Properties
  x-api-slug: google-analytics
  description: Lists web properties to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties
  tags: Web Property
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebproperties-get-openapi.md
- name: Google Analytics Create Web Property
  x-api-slug: google-analytics
  description: Create a new property if the account has fewer than 20 properties.
    Web properties are visible in the Google Analytics interface only if they have
    at least one profile.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties
  tags: Web Property
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebproperties-post-openapi.md
- name: Google Analytics Get Web Property
  x-api-slug: google-analytics
  description: Gets a web property to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}
  tags: Web Property
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyid-get-openapi.md
- name: Google Analytics Update Web Property
  x-api-slug: google-analytics
  description: Updates an existing web property. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}
  tags: Web Property
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyid-patch-openapi.md
- name: Google Analytics Update Web Property
  x-api-slug: google-analytics
  description: Updates an existing web property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}
  tags: Web Property
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyid-put-openapi.md
- name: Google Analytics Get Custom Data
  x-api-slug: google-analytics
  description: List custom data sources to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customDataSources
  tags: Custom Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdatasources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdatasources-get-openapi.md
- name: Google Analytics Delete Data
  x-api-slug: google-analytics
  description: Delete data associated with a previous upload.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customDataSources/{customDataSourceId}/deleteUploadData
  tags: Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdatasourcescustomdatasourceiddeleteuploaddata-post-openapi.md
- name: Google Analytics List Uploads
  x-api-slug: google-analytics
  description: List uploads to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customDataSources/{customDataSourceId}/uploads
  tags: Upload
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdatasourcescustomdatasourceiduploads-get-openapi.md
- name: Google Analytics Upload Data
  x-api-slug: google-analytics
  description: Upload data for a custom data source.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customDataSources/{customDataSourceId}/uploads
  tags: Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdatasourcescustomdatasourceiduploads-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdatasourcescustomdatasourceiduploads-post-openapi.md
- name: Google Analytics Get UPloads
  x-api-slug: google-analytics
  description: List uploads to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customDataSources/{customDataSourceId}/uploads/{uploadId}
  tags: Upload
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdatasourcescustomdatasourceiduploadsuploadid-get-openapi.md
- name: Google Analytics Get Custom Dimensions
  x-api-slug: google-analytics
  description: Lists custom dimensions to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customDimensions
  tags: Dimension
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdimensions-get-openapi.md
- name: Google Analytics Create Custom Dimension
  x-api-slug: google-analytics
  description: Create a new custom dimension.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customDimensions
  tags: Dimension
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdimensions-post-openapi.md
- name: Google Analytics Get Custom Dimension
  x-api-slug: google-analytics
  description: Get a custom dimension to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customDimensions/{customDimensionId}
  tags: Dimension
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdimensionscustomdimensionid-get-openapi.md
- name: Google Analytics Update Custom Dimensions
  x-api-slug: google-analytics
  description: Updates an existing custom dimension. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customDimensions/{customDimensionId}
  tags: Dimension
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdimensionscustomdimensionid-patch-openapi.md
- name: Google Analytics Update Custom Dimensions
  x-api-slug: google-analytics
  description: Updates an existing custom dimension.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customDimensions/{customDimensionId}
  tags: Dimension
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustomdimensionscustomdimensionid-put-openapi.md
- name: Google Analytics Get Custom Metrics
  x-api-slug: google-analytics
  description: Lists custom metrics to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customMetrics
  tags: Metric
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustommetrics-get-openapi.md
- name: Google Analytics Create Custom Metric
  x-api-slug: google-analytics
  description: Create a new custom metric.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customMetrics
  tags: Metric
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustommetrics-post-openapi.md
- name: Google Analytics Get Custom Metric
  x-api-slug: google-analytics
  description: Get a custom metric to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customMetrics/{customMetricId}
  tags: Metric
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustommetricscustommetricid-get-openapi.md
- name: Google Analytics Update Custom Metric
  x-api-slug: google-analytics
  description: Updates an existing custom metric. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customMetrics/{customMetricId}
  tags: Metric
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustommetricscustommetricid-patch-openapi.md
- name: Google Analytics Update Custom Metric
  x-api-slug: google-analytics
  description: Updates an existing custom metric.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/customMetrics/{customMetricId}
  tags: Metric
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidcustommetricscustommetricid-put-openapi.md
- name: Google Analytics List AdWords
  x-api-slug: google-analytics
  description: Lists webProperty-AdWords links for a given web property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/entityAdWordsLinks
  tags: AdWord
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinks-get-openapi.md
- name: Google Analytics Create AdWord
  x-api-slug: google-analytics
  description: Creates a webProperty-AdWords link.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/entityAdWordsLinks
  tags: AdWord
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinks-post-openapi.md
- name: Google Analytics Delete AdWord
  x-api-slug: google-analytics
  description: Deletes a web property-AdWords link.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/entityAdWordsLinks/{webPropertyAdWordsLinkId}
  tags: AdWord
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinkswebpropertyadwordslinkid-delete-openapi.md
- name: Google Analytics Get AdWord
  x-api-slug: google-analytics
  description: Returns a web property-AdWords link to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/entityAdWordsLinks/{webPropertyAdWordsLinkId}
  tags: AdWord
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinkswebpropertyadwordslinkid-get-openapi.md
- name: Google Analytics Update AdWord
  x-api-slug: google-analytics
  description: Updates an existing webProperty-AdWords link. This method supports
    patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/entityAdWordsLinks/{webPropertyAdWordsLinkId}
  tags: AdWord
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinkswebpropertyadwordslinkid-patch-openapi.md
- name: Google Analytics Update AdWord
  x-api-slug: google-analytics
  description: Updates an existing webProperty-AdWords link.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/entityAdWordsLinks/{webPropertyAdWordsLinkId}
  tags: AdWord
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidentityadwordslinkswebpropertyadwordslinkid-put-openapi.md
- name: Google Analytics Get Users
  x-api-slug: google-analytics
  description: Lists webProperty-user links for a given web property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/entityUserLinks
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidentityuserlinks-get-openapi.md
- name: Google Analytics Add User
  x-api-slug: google-analytics
  description: Adds a new user to the given web property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/entityUserLinks
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidentityuserlinks-post-openapi.md
- name: Google Analytics Remove User
  x-api-slug: google-analytics
  description: Removes a user from the given web property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/entityUserLinks/{linkId}
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidentityuserlinkslinkid-delete-openapi.md
- name: Google Analytics Update Permission
  x-api-slug: google-analytics
  description: Updates permissions for an existing user on the given web property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/entityUserLinks/{linkId}
  tags: Permission
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidentityuserlinkslinkid-put-openapi.md
- name: Google Analytics List Views
  x-api-slug: google-analytics
  description: Lists views (profiles) to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles
  tags: View
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofiles-get-openapi.md
- name: Google Analytics Create View
  x-api-slug: google-analytics
  description: Create a new view (profile).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles
  tags: View
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofiles-post-openapi.md
- name: Google Analytics Delete View
  x-api-slug: google-analytics
  description: Deletes a view (profile).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}
  tags: View
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileid-delete-openapi.md
- name: Google Analytics Get View
  x-api-slug: google-analytics
  description: Gets a view (profile) to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}
  tags: View
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileid-get-openapi.md
- name: Google Analytics Update View
  x-api-slug: google-analytics
  description: Updates an existing view (profile). This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}
  tags: View
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileid-patch-openapi.md
- name: Google Analytics Update View
  x-api-slug: google-analytics
  description: Updates an existing view (profile).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}
  tags: View
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileid-put-openapi.md
- name: Google Analytics List Users
  x-api-slug: google-analytics
  description: Lists profile-user links for a given view (profile).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/entityUserLinks
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidentityuserlinks-get-openapi.md
- name: Google Analytics Add User
  x-api-slug: google-analytics
  description: Adds a new user to the given view (profile).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/entityUserLinks
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidentityuserlinks-post-openapi.md
- name: Google Analytics Remove User
  x-api-slug: google-analytics
  description: Removes a user from the given view (profile).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/entityUserLinks/{linkId}
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidentityuserlinkslinkid-delete-openapi.md
- name: Google Analytics Update Permissions
  x-api-slug: google-analytics
  description: Updates permissions for an existing user on the given view (profile).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/entityUserLinks/{linkId}
  tags: Permission
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidentityuserlinkslinkid-put-openapi.md
- name: Google Analytics List Experiments
  x-api-slug: google-analytics
  description: Lists experiments to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/experiments
  tags: Experiment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperiments-get-openapi.md
- name: Google Analytics Create Experiment
  x-api-slug: google-analytics
  description: Create a new experiment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/experiments
  tags: Experiment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperiments-post-openapi.md
- name: Google Analytics Delete Experiment
  x-api-slug: google-analytics
  description: Delete an experiment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/experiments/{experimentId}
  tags: Experiment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperimentsexperimentid-delete-openapi.md
- name: Google Analytics Get Experiment
  x-api-slug: google-analytics
  description: Returns an experiment to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/experiments/{experimentId}
  tags: Experiment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperimentsexperimentid-get-openapi.md
- name: Google Analytics Update Experiment
  x-api-slug: google-analytics
  description: Update an existing experiment. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/experiments/{experimentId}
  tags: Experiment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperimentsexperimentid-patch-openapi.md
- name: Google Analytics Update Experiment
  x-api-slug: google-analytics
  description: Update an existing experiment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/experiments/{experimentId}
  tags: Experiment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidexperimentsexperimentid-put-openapi.md
- name: Google Analytics Get Goals
  x-api-slug: google-analytics
  description: Lists goals to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/goals
  tags: Goal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidgoals-get-openapi.md
- name: Google Analytics Create Goal
  x-api-slug: google-analytics
  description: Create a new goal.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/goals
  tags: Goal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidgoals-post-openapi.md
- name: Google Analytics Get Goal
  x-api-slug: google-analytics
  description: Gets a goal to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/goals/{goalId}
  tags: Goal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidgoalsgoalid-get-openapi.md
- name: Google Analytics Update Goal
  x-api-slug: google-analytics
  description: Updates an existing goal. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/goals/{goalId}
  tags: Goal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidgoalsgoalid-patch-openapi.md
- name: Google Analytics Update Goal
  x-api-slug: google-analytics
  description: Updates an existing goal.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/goals/{goalId}
  tags: Goal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidgoalsgoalid-put-openapi.md
- name: Google Analytics Get Profile Filter
  x-api-slug: google-analytics
  description: Lists all profile filter links for a profile.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/profileFilterLinks
  tags: Profile Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinks-get-openapi.md
- name: Google Analytics Create Profile Filter
  x-api-slug: google-analytics
  description: Create a new profile filter link.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/profileFilterLinks
  tags: Profile Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinks-post-openapi.md
- name: Google Analytics Delete Profile Filter
  x-api-slug: google-analytics
  description: Delete a profile filter link.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/profileFilterLinks/{linkId}
  tags: Profile Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinkslinkid-delete-openapi.md
- name: Google Analytics Get Profile Filter
  x-api-slug: google-analytics
  description: Returns a single profile filter link.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/profileFilterLinks/{linkId}
  tags: Profile Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinkslinkid-get-openapi.md
- name: Google Analytics Update Profile Filter
  x-api-slug: google-analytics
  description: Update an existing profile filter link. This method supports patch
    semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/profileFilterLinks/{linkId}
  tags: Profile Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinkslinkid-patch-openapi.md
- name: Google Analytics Update Profile Filter
  x-api-slug: google-analytics
  description: Update an existing profile filter link.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/profileFilterLinks/{linkId}
  tags: Profile Filter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinkslinkid-put-openapi.md
- name: Google Analytics Get Unsampled Reports
  x-api-slug: google-analytics
  description: Lists unsampled reports to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/unsampledReports
  tags: Report
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidunsampledreports-get-openapi.md
- name: Google Analytics Create Unsampled Report
  x-api-slug: google-analytics
  description: Create a new unsampled report.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/unsampledReports
  tags: Report
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidunsampledreports-post-openapi.md
- name: Google Analytics Delete Unsampled Report
  x-api-slug: google-analytics
  description: Deletes an unsampled report.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/unsampledReports/{unsampledReportId}
  tags: Report
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidunsampledreportsunsampledreportid-delete-openapi.md
- name: Google Analytics Get Unsampled Report
  x-api-slug: google-analytics
  description: Returns a single unsampled report.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/unsampledReports/{unsampledReportId}
  tags: Report
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidunsampledreportsunsampledreportid-get-openapi.md
- name: Google Analytics Get Remarketing Audiences
  x-api-slug: google-analytics
  description: Lists remarketing audiences to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/remarketingAudiences
  tags: Remarketing Audience
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidremarketingaudiences-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidremarketingaudiences-get-openapi.md
- name: Google Analytics Create Remarketing Audience
  x-api-slug: google-analytics
  description: Creates a new remarketing audience.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/remarketingAudiences
  tags: Remarketing Audience
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidremarketingaudiences-post-openapi.md
- name: Google Analytics Get Remarketing Audience
  x-api-slug: google-analytics
  description: Gets a remarketing audience to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/remarketingAudiences/{remarketingAudienceId}
  tags: Remarketing Audience
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidremarketingaudiencesremarketingaudienceid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidremarketingaudiencesremarketingaudienceid-get-openapi.md
- name: Google Analytics Update Remarketing Audience
  x-api-slug: google-analytics
  description: Updates an existing remarketing audience. This method supports patch
    semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/remarketingAudiences/{remarketingAudienceId}
  tags: Remarketing Audience
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidremarketingaudiencesremarketingaudienceid-patch-openapi.md
- name: Google Analytics Update Remarketing Audience
  x-api-slug: google-analytics
  description: Updates an existing remarketing audience.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/accounts/{accountId}/webproperties/{webPropertyId}/remarketingAudiences/{remarketingAudienceId}
  tags: Remarketing Audience
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementaccountsaccountidwebpropertieswebpropertyidremarketingaudiencesremarketingaudienceid-put-openapi.md
- name: Google Analytics Get Segments
  x-api-slug: google-analytics
  description: Lists segments to which the user has access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//management/segments
  tags: Segment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/managementsegments-get-openapi.md
- name: Google Analytics Get Columsn
  x-api-slug: google-analytics
  description: Lists all columns for a report type
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//metadata/{reportType}/columns
  tags: Column
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/metadatareporttypecolumns-get-openapi.md
- name: Google Analytics Create Account Ticket
  x-api-slug: google-analytics
  description: Creates an account ticket.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3//provisioning/createAccountTicket
  tags: Tickets
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/provisioningcreateaccountticket-post-openapi.md
- name: Google Analytics
  x-api-slug: google-analytics
  description: Google Analytics gives you the digital analytics tools you need to
    analyze data from all touchpoints in one place, for a deeper understanding of
    the customer experience. You can then share the insights that matter with your
    whole organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logo_lockup_analytics_icon_vertical_black_2x.png
  humanURL: https://www.google.com/analytics/#?modal_active=none
  baseURL: https://www.googleapis.com//analytics/v3
  tags: Google Analytics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-analytics/master/_listings/google-analytics/openapi.md
x-common:
- type: x-blog
  url: https://analytics.googleblog.com/
- type: x-blog-rss
  url: https://analytics.googleblog.com/feeds/posts/default?alt=rss
- type: x-developer
  url: https://developers.google.com/analytics/
- type: x-github
  url: https://github.com/googleanalytics/
- type: x-google-plus
  url: https://plus.google.com/+GoogleAnalytics
- type: x-partners
  url: https://developers.google.com/analytics/program/
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/google-analytics
- type: x-support
  url: https://developers.google.com/analytics/help/
- type: x-twitter
  url: https://twitter.com/googleanalytics
- type: x-videos
  url: https://www.youtube.com/user/googleanalytics
- type: x-website
  url: https://www.google.com/analytics/#?modal_active=none
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---