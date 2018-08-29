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
created: "2018-08-29"
modified: "2018-08-29"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Advisor API - Generate Recommendations
  x-api-slug: subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendations-post
  description: Initiates the recommendation generation or computation process for
    a subscription. This operation is asynchronous. The generated recommendations
    are stored in a cache in the Advisor service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com//
  tags: Best Practices, Performance, Microsoft, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendations-post-openapi.md
- name: Azure Advisor API - Get Recommendation
  x-api-slug: subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendationsoperationid-get
  description: Retrieves the status of the recommendation computation or generation
    process. Invoke this API after calling the generation recommendation. The URI
    of this API is returned in the Location field of the response header.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com//
  tags: Best Practices, Performance, Microsoft, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendationsoperationid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorgeneraterecommendationsoperationid-get-openapi.md
- name: Azure Advisor API - List Recommendations
  x-api-slug: subscriptionssubscriptionidprovidersmicrosoft-advisorrecommendations-get
  description: Obtains cached recommendations for a subscription. The recommendations
    are generated or computed by invoking generateRecommendations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com//
  tags: Best Practices, Performance, Microsoft, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorrecommendations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorrecommendations-get-openapi.md
- name: Azure Advisor API - List Operations
  x-api-slug: providersmicrosoft-advisoroperations-get
  description: Lists all the available Advisor REST API operations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com//
  tags: Best Practices, Performance, Microsoft, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/providersmicrosoft-advisoroperations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/providersmicrosoft-advisoroperations-get-openapi.md
- name: Azure Advisor API - Get Suppressions
  x-api-slug: resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-get
  description: Obtains the details of a suppression.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com//
  tags: Best Practices, Performance, Microsoft, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-get-openapi.md
- name: Azure Advisor API - Create Suppressions
  x-api-slug: resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-put
  description: Enables the snoozed or dismissed attribute of a recommendation. The
    snoozed or dismissed attribute is referred to as a suppression. Use this API to
    create or update the snoozed or dismissed status of a recommendation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com//
  tags: Best Practices, Performance, Microsoft, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-put-openapi.md
- name: Azure Advisor API - Delete Suppressions
  x-api-slug: resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-delete
  description: Enables the activation of a snoozed or dismissed recommendation. The
    snoozed or dismissed attribute of a recommendation is referred to as a suppression.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com//
  tags: Best Practices, Performance, Microsoft, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationidsuppressionsname-delete-openapi.md
- name: Azure Advisor API - Get Recommendations
  x-api-slug: resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationid-get
  description: Obtains details of a cached recommendation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com//
  tags: Best Practices, Performance, Microsoft, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/resourceuriprovidersmicrosoft-advisorrecommendationsrecommendationid-get-openapi.md
- name: Azure Advisor API - List Suppressions
  x-api-slug: subscriptionssubscriptionidprovidersmicrosoft-advisorsuppressions-get
  description: Retrieves the list of snoozed or dismissed suppressions for a subscription.
    The snoozed or dismissed attribute of a recommendation is referred to as a suppression.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/improve-what-matters.png
  humanURL: https://azure.microsoft.com/en-us/services/advisor/
  baseURL: ://management.azure.com//
  tags: Best Practices, Performance, Microsoft, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-advisor/master/_listings/azure-advisor/subscriptionssubscriptionidprovidersmicrosoft-advisorsuppressions-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aylien.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.advisor.stack.network
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