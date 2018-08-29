---
swagger: "2.0"
x-collection-name: Azure Advisor
x-complete: 0
info:
  title: Azure Advisor API List Operations
  description: Lists all the available Advisor REST API operations.
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
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftadvisorgeneraterecommendations-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Recommendations
  /subscriptions/{subscriptionId}/providers/Microsoft.Advisor/generateRecommendations/{operationId}:
    get:
      summary: Get Recommendation
      description: Retrieves the status of the recommendation computation or generation
        process. Invoke this API after calling the generation recommendation. The
        URI of this API is returned in the Location field of the response header.
      operationId: Recommendations_GetGenerateStatus
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftadvisorgeneraterecommendationsoperationid-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: operationId
        description: The operation ID, which can be found from the Location field
          in the generate recommendation response header
      responses:
        200:
          description: OK
      tags:
      - Recommendations
  /subscriptions/{subscriptionId}/providers/Microsoft.Advisor/recommendations:
    get:
      summary: List Recommendations
      description: Obtains cached recommendations for a subscription. The recommendations
        are generated or computed by invoking generateRecommendations.
      operationId: Recommendations_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftadvisorrecommendations-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply to the recommendations
      - in: query
        name: $skipToken
        description: The page-continuation token to use with a paged version of this
          API
      - in: query
        name: $top
        description: The number of recommendations per page if a paged version of
          this API is being used
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Recommendations
  /providers/Microsoft.Advisor/operations:
    get:
      summary: List Operations
      description: Lists all the available Advisor REST API operations.
      operationId: Operations_List
      x-api-path-slug: providersmicrosoftadvisoroperations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Operations
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