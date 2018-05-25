---
swagger: "2.0"
x-collection-name: Azure Advisor
x-complete: 0
info:
  title: Azure Advisor API List Suppressions
  description: Retrieves the list of snoozed or dismissed suppressions for a subscription.
    The snoozed or dismissed attribute of a recommendation is referred to as a suppression.
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
  /subscriptions/{subscriptionId}/providers/Microsoft.Advisor/generateRecommendations/{operationId}:
    get:
      summary: Get Recommendation
      description: Retrieves the status of the recommendation computation or generation
        process. Invoke this API after calling the generation recommendation. The
        URI of this API is returned in the Location field of the response header.
      operationId: Recommendations_GetGenerateStatus
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendationsoperationid-get
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
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-advisorrecommendations-get
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
      x-api-path-slug: providersmicrosoft-advisoroperations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Operations
  /{resourceUri}/providers/Microsoft.Advisor/recommendations/{recommendationId}/suppressions/{name}:
    get:
      summary: Get Suppressions
      description: Obtains the details of a suppression.
      operationId: Suppressions_Get
      x-api-path-slug: resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-get
      parameters:
      - in: path
        name: name
        description: The name of the suppression
      - in: query
        name: No Name
      - in: path
        name: recommendationId
        description: The recommendation ID
      - in: path
        name: resourceUri
        description: The fully qualified Azure Resource Manager identifier of the
          resource to which the recommendation applies
      responses:
        200:
          description: OK
      tags:
      - Suppressions
    put:
      summary: Create Suppressions
      description: Enables the snoozed or dismissed attribute of a recommendation.
        The snoozed or dismissed attribute is referred to as a suppression. Use this
        API to create or update the snoozed or dismissed status of a recommendation.
      operationId: Suppressions_Create
      x-api-path-slug: resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-put
      parameters:
      - in: path
        name: name
        description: The name of the suppression
      - in: query
        name: No Name
      - in: path
        name: recommendationId
        description: The recommendation ID
      - in: path
        name: resourceUri
        description: The fully qualified Azure Resource Manager identifier of the
          resource to which the recommendation applies
      - in: body
        name: suppressionContract
        description: The snoozed or dismissed attribute; for example, the snooze duration
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Suppressions
    delete:
      summary: Delete Suppressions
      description: Enables the activation of a snoozed or dismissed recommendation.
        The snoozed or dismissed attribute of a recommendation is referred to as a
        suppression.
      operationId: Suppressions_Delete
      x-api-path-slug: resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-delete
      parameters:
      - in: path
        name: name
        description: The name of the suppression
      - in: query
        name: No Name
      - in: path
        name: recommendationId
        description: The recommendation ID
      - in: path
        name: resourceUri
        description: The fully qualified Azure Resource Manager identifier of the
          resource to which the recommendation applies
      responses:
        200:
          description: OK
      tags:
      - Suppressions
  /{resourceUri}/providers/Microsoft.Advisor/recommendations/{recommendationId}:
    get:
      summary: Get Recommendations
      description: Obtains details of a cached recommendation.
      operationId: Recommendations_Get
      x-api-path-slug: resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationid-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: recommendationId
        description: The recommendation ID
      - in: path
        name: resourceUri
        description: The fully qualified Azure Resource Manager identifier of the
          resource to which the recommendation applies
      responses:
        200:
          description: OK
      tags:
      - Recommendations
  /subscriptions/{subscriptionId}/providers/Microsoft.Advisor/suppressions:
    get:
      summary: List Suppressions
      description: Retrieves the list of snoozed or dismissed suppressions for a subscription.
        The snoozed or dismissed attribute of a recommendation is referred to as a
        suppression.
      operationId: Suppressions_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-advisorsuppressions-get
      parameters:
      - in: query
        name: $skipToken
        description: The page-continuation token to use with a paged version of this
          API
      - in: query
        name: $top
        description: The number of suppressions per page if a paged version of this
          API is being used
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Suppressions
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