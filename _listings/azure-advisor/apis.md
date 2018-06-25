---
name: Azure Advisor
x-slug: azure-advisor
description: Azure Advisor is a personalized recommendation engine that helps you
  follow Azure best practices. It analyzes your Azure resource configuration and usage
  telemetry, then provides recommendations that can reduce costs and improve the performance,
  security, and reliability of your applications.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Azure Advisor
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Advisor API Generate Recommendations
  x-api-slug: azure-advisor-api
  description: Initiates the recommendation generation or computation process for
    a subscription. This operation is asynchronous. The generated recommendations
    are stored in a cache in the Advisor service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Advisor/generateRecommendations
  tags: Recommendations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendations-post-openapi.md
- name: Azure Advisor API Get Recommendation
  x-api-slug: azure-advisor-api
  description: Retrieves the status of the recommendation computation or generation
    process. Invoke this API after calling the generation recommendation. The URI
    of this API is returned in the Location field of the response header.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Advisor/generateRecommendations/{operationId}
  tags: Recommendations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendationsoperationid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendationsoperationid-get-openapi.md
- name: Azure Advisor API List Recommendations
  x-api-slug: azure-advisor-api
  description: Obtains cached recommendations for a subscription. The recommendations
    are generated or computed by invoking generateRecommendations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Advisor/recommendations
  tags: Recommendations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorrecommendations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorrecommendations-get-openapi.md
- name: Azure Advisor API List Operations
  x-api-slug: azure-advisor-api
  description: Lists all the available Advisor REST API operations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com////providers/Microsoft.Advisor/operations
  tags: Operations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/providersmicrosoft-advisoroperations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/providersmicrosoft-advisoroperations-get-openapi.md
- name: Azure Advisor API Get Suppressions
  x-api-slug: azure-advisor-api
  description: Obtains the details of a suppression.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com////{resourceUri}/providers/Microsoft.Advisor/recommendations/{recommendationId}/suppressions/{name}
  tags: Suppressions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-get-openapi.md
- name: Azure Advisor API Create Suppressions
  x-api-slug: azure-advisor-api
  description: Enables the snoozed or dismissed attribute of a recommendation. The
    snoozed or dismissed attribute is referred to as a suppression. Use this API to
    create or update the snoozed or dismissed status of a recommendation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com////{resourceUri}/providers/Microsoft.Advisor/recommendations/{recommendationId}/suppressions/{name}
  tags: Suppressions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-put-openapi.md
- name: Azure Advisor API Delete Suppressions
  x-api-slug: azure-advisor-api
  description: Enables the activation of a snoozed or dismissed recommendation. The
    snoozed or dismissed attribute of a recommendation is referred to as a suppression.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com////{resourceUri}/providers/Microsoft.Advisor/recommendations/{recommendationId}/suppressions/{name}
  tags: Suppressions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-delete-openapi.md
- name: Azure Advisor API Get Recommendations
  x-api-slug: azure-advisor-api
  description: Obtains details of a cached recommendation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com////{resourceUri}/providers/Microsoft.Advisor/recommendations/{recommendationId}
  tags: Recommendations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationid-get-openapi.md
- name: Azure Advisor API List Suppressions
  x-api-slug: azure-advisor-api
  description: Retrieves the list of snoozed or dismissed suppressions for a subscription.
    The snoozed or dismissed attribute of a recommendation is referred to as a suppression.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Advisor/suppressions
  tags: Suppressions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorsuppressions-get-openapi.md
- name: Azure Advisor API
  x-api-slug: azure-advisor-api
  description: Azure Advisor is a personalized recommendation engine that helps you
    follow Azure best practices. It analyzes your Azure resource configuration and
    usage telemetry, then provides recommendations that can reduce costs and improve
    the performance, security, and reliability of your applications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com//
  tags: Azure Advisor
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/advisor/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/advisor/
- type: x-regions
  url: https://azure.microsoft.com/en-us/status/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/advisor/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/advisor/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---