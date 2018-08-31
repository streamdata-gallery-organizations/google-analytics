---
swagger: "2.0"
info:
  title: Google Analytics
  description: Views and manages your Google Analytics data.
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
  /management/accounts/{accountId}/webproperties/{webPropertyId}/remarketingAudiences/{remarketingAudienceId}:
    put:
      summary: Update Remarketing Audience
      description: Updates an existing remarketing audience
      operationId: analytics.management.remarketingAudience.update
      parameters:
      - in: path
        name: accountId
        description: The account ID of the remarketing audience to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: remarketingAudienceId
        description: The ID of the remarketing audience to update
      - in: path
        name: webPropertyId
        description: The web property ID of the remarketing audience to update
      responses:
        200:
          description: OK
      tags:
      - remarketing audience
definitions:
  Account:
    properties:
      childLink:
        description: This is a default description.
        type: post
      created:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      permissions:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
      starred:
        description: This is a default description.
        type: post
      updated:
        description: This is a default description.
        type: post
  AccountRef:
    properties:
      href:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  AccountSummaries:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  AccountSummary:
    properties:
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      starred:
        description: This is a default description.
        type: post
      webProperties:
        description: This is a default description.
        type: post
  AccountTicket:
    properties:
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      redirectUri:
        description: This is a default description.
        type: post
  Accounts:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  AdWordsAccount:
    properties:
      autoTaggingEnabled:
        description: This is a default description.
        type: post
      customerId:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  AnalyticsDataimportDeleteUploadDataRequest:
    properties:
      customDataImportUids:
        description: This is a default description.
        type: post
  Column:
    properties:
      attributes:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  Columns:
    properties:
      attributeNames:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
  CustomDataSource:
    properties:
      accountId:
        description: This is a default description.
        type: post
      childLink:
        description: This is a default description.
        type: post
      created:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      importBehavior:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      parentLink:
        description: This is a default description.
        type: post
      profilesLinked:
        description: This is a default description.
        type: post
  CustomDataSources:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  CustomDimension:
    properties:
      accountId:
        description: This is a default description.
        type: post
      active:
        description: This is a default description.
        type: post
      created:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      index:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      parentLink:
        description: This is a default description.
        type: post
      scope:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  CustomDimensions:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  CustomMetric:
    properties:
      accountId:
        description: This is a default description.
        type: post
      active:
        description: This is a default description.
        type: post
      created:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      index:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      max_value:
        description: This is a default description.
        type: post
      min_value:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      parentLink:
        description: This is a default description.
        type: post
  CustomMetrics:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  EntityAdWordsLink:
    properties:
      adWordsAccounts:
        description: This is a default description.
        type: post
      entity:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      profileIds:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  EntityAdWordsLinks:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
  EntityUserLink:
    properties:
      entity:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      permissions:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  EntityUserLinks:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
  Experiment:
    properties:
      accountId:
        description: This is a default description.
        type: post
      created:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      editableInGaUi:
        description: This is a default description.
        type: post
      endTime:
        description: This is a default description.
        type: post
      equalWeighting:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      internalWebPropertyId:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      minimumExperimentLengthInDays:
        description: This is a default description.
        type: post
  Experiments:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  Filter:
    properties:
      accountId:
        description: This is a default description.
        type: post
      advancedDetails:
        description: This is a default description.
        type: post
      created:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      lowercaseDetails:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      parentLink:
        description: This is a default description.
        type: post
      searchAndReplaceDetails:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  FilterExpression:
    properties:
      caseSensitive:
        description: This is a default description.
        type: post
      expressionValue:
        description: This is a default description.
        type: post
      field:
        description: This is a default description.
        type: post
      fieldIndex:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      matchType:
        description: This is a default description.
        type: post
  FilterRef:
    properties:
      accountId:
        description: This is a default description.
        type: post
      href:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  Filters:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  GaData:
    properties:
      columnHeaders:
        description: This is a default description.
        type: post
      containsSampledData:
        description: This is a default description.
        type: post
      dataLastRefreshed:
        description: This is a default description.
        type: post
      dataTable:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      profileInfo:
        description: This is a default description.
        type: post
  Goal:
    properties:
      accountId:
        description: This is a default description.
        type: post
      active:
        description: This is a default description.
        type: post
      created:
        description: This is a default description.
        type: post
      eventDetails:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      internalWebPropertyId:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      parentLink:
        description: This is a default description.
        type: post
      profileId:
        description: This is a default description.
        type: post
  Goals:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  IncludeConditions:
    properties:
      daysToLookBack:
        description: This is a default description.
        type: post
      isSmartList:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      membershipDurationDays:
        description: This is a default description.
        type: post
      segment:
        description: This is a default description.
        type: post
  LinkedForeignAccount:
    properties:
      accountId:
        description: This is a default description.
        type: post
      eligibleForSearch:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      internalWebPropertyId:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      linkedAccountId:
        description: This is a default description.
        type: post
      remarketingAudienceId:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
      webPropertyId:
        description: This is a default description.
        type: post
  McfData:
    properties:
      columnHeaders:
        description: This is a default description.
        type: post
      containsSampledData:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      profileInfo:
        description: This is a default description.
        type: post
      query:
        description: This is a default description.
        type: post
      rows:
        description: This is a default description.
        type: post
  Profile:
    properties:
      accountId:
        description: This is a default description.
        type: post
      botFilteringEnabled:
        description: This is a default description.
        type: post
      childLink:
        description: This is a default description.
        type: post
      created:
        description: This is a default description.
        type: post
      currency:
        description: This is a default description.
        type: post
      defaultPage:
        description: This is a default description.
        type: post
      eCommerceTracking:
        description: This is a default description.
        type: post
      enhancedECommerceTracking:
        description: This is a default description.
        type: post
      excludeQueryParameters:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
  ProfileFilterLink:
    properties:
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      rank:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  ProfileFilterLinks:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  ProfileRef:
    properties:
      accountId:
        description: This is a default description.
        type: post
      href:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      internalWebPropertyId:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      webPropertyId:
        description: This is a default description.
        type: post
  ProfileSummary:
    properties:
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      starred:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  Profiles:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  RealtimeData:
    properties:
      columnHeaders:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      profileInfo:
        description: This is a default description.
        type: post
      query:
        description: This is a default description.
        type: post
      rows:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      totalsForAllResults:
        description: This is a default description.
        type: post
  RemarketingAudience:
    properties:
      accountId:
        description: This is a default description.
        type: post
      audienceDefinition:
        description: This is a default description.
        type: post
      audienceType:
        description: This is a default description.
        type: post
      created:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      internalWebPropertyId:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      linkedAdAccounts:
        description: This is a default description.
        type: post
      linkedViews:
        description: This is a default description.
        type: post
  RemarketingAudiences:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  Segment:
    properties:
      created:
        description: This is a default description.
        type: post
      definition:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      segmentId:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
      updated:
        description: This is a default description.
        type: post
  Segments:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  UnsampledReport:
    properties:
      accountId:
        description: This is a default description.
        type: post
      cloudStorageDownloadDetails:
        description: This is a default description.
        type: post
      created:
        description: This is a default description.
        type: post
      dimensions:
        description: This is a default description.
        type: post
      downloadType:
        description: This is a default description.
        type: post
      driveDownloadDetails:
        description: This is a default description.
        type: post
      end-date:
        description: This is a default description.
        type: post
      filters:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  UnsampledReports:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  Upload:
    properties:
      accountId:
        description: This is a default description.
        type: post
      customDataSourceId:
        description: This is a default description.
        type: post
      errors:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
  Uploads:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
  UserRef:
    properties:
      email:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  WebPropertyRef:
    properties:
      accountId:
        description: This is a default description.
        type: post
      href:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      internalWebPropertyId:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  WebPropertySummary:
    properties:
      id:
        description: This is a default description.
        type: post
      internalWebPropertyId:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      level:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      profiles:
        description: This is a default description.
        type: post
      starred:
        description: This is a default description.
        type: post
      websiteUrl:
        description: This is a default description.
        type: post
  Webproperties:
    properties:
      items:
        description: This is a default description.
        type: post
      itemsPerPage:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
      previousLink:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  Webproperty:
    properties:
      accountId:
        description: This is a default description.
        type: post
      childLink:
        description: This is a default description.
        type: post
      created:
        description: This is a default description.
        type: post
      defaultProfileId:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      industryVertical:
        description: This is a default description.
        type: post
      internalWebPropertyId:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      level:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
x-collection-name: Google Analytics
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