---
swagger: "2.0"
x-collection-name: Google Analytics
x-complete: 0
info:
  title: Google Analytics Return Real Time Data
  description: Returns real time data for a view (profile).
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