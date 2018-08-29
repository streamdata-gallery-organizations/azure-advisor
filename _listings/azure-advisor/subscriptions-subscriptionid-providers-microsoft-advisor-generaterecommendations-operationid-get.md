---
swagger: "2.0"
info:
  title: Azure Advisor API
  description: Azure Advisor is a personalized recommendation engine that helps you
    follow Azure best practices. It analyzes your Azure resource configuration and
    usage telemetry, then provides recommendations that can reduce costs and improve
    the performance, security, and reliability of your applications.
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
  /subscriptions/{subscriptionId}/providers/Microsoft.Advisor/generateRecommendations/{operationId}:
    get:
      summary: Get Recommendation
      description: Retrieves the status of the recommendation computation or generation
        process
      operationId: Recommendations_GetGenerateStatus
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
      - recommendations
definitions:
  ResourceRecommendationBaseListResult:
    properties:
      nextLink:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
  ResourceRecommendationBase:
    properties: []
  RecommendationProperties:
    properties:
      category:
        description: This is a default description.
        type: get
      impact:
        description: This is a default description.
        type: get
      impactedField:
        description: This is a default description.
        type: get
      impactedValue:
        description: This is a default description.
        type: get
      lastUpdated:
        description: This is a default description.
        type: get
      metadata:
        description: This is a default description.
        type: get
      recommendationTypeId:
        description: This is a default description.
        type: get
      risk:
        description: This is a default description.
        type: get
      suppressionIds:
        description: This is a default description.
        type: get
  Resource:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  ShortDescription:
    properties:
      problem:
        description: This is a default description.
        type: get
      solution:
        description: This is a default description.
        type: get
  OperationEntityListResult:
    properties:
      nextLink:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
  OperationEntity:
    properties:
      name:
        description: This is a default description.
        type: get
  OperationDisplayInfo:
    properties:
      description:
        description: This is a default description.
        type: get
      operation:
        description: This is a default description.
        type: get
      provider:
        description: This is a default description.
        type: get
      resource:
        description: This is a default description.
        type: get
  SuppressionContract:
    properties: []
  SuppressionProperties:
    properties:
      suppressionId:
        description: This is a default description.
        type: get
      ttl:
        description: This is a default description.
        type: get
  SuppressionContractListResult:
    properties:
      nextLink:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
x-collection-name: Azure Advisor
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