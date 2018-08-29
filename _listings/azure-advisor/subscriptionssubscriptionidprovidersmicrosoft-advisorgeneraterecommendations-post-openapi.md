---
swagger: "2.0"
x-collection-name: Azure Advisor
x-complete: 0
info:
  title: Azure Advisor API Generate Recommendations
  description: Initiates the recommendation generation or computation process for
    a subscription. This operation is asynchronous. The generated recommendations
    are stored in a cache in the Advisor service.
  version: "2017-04-19"
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.Advisor/generateRecommendations:
    post:
      summary: Generate Recommendations
      description: Initiates the recommendation generation or computation process
        for a subscription. This operation is asynchronous. The generated recommendations
        are stored in a cache in the Advisor service.
      operationId: Recommendations_Generate
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendations-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Recommendations
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