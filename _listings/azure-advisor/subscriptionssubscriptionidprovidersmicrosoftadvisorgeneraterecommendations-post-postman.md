{
  "info": {
    "name": "Azure Advisor API Generate Recommendations",
    "_postman_id": "cf850ebe-4075-40fd-8bc8-f2413f72a4af",
    "description": "Initiates the recommendation generation or computation process for a subscription. This operation is asynchronous. The generated recommendations are stored in a cache in the Advisor service.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "recommendations",
      "item": [
        {
          "id": "ae3f8cd5-9e35-4da6-bd02-ca1cd6b3fa93",
          "name": "Recommendations_Generate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Advisor/generateRecommendations"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates the recommendation generation or computation process for a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "635a5a72-1e3b-42bf-aff7-097970f3a5cf"
            }
          ]
        }
      ]
    }
  ]
}