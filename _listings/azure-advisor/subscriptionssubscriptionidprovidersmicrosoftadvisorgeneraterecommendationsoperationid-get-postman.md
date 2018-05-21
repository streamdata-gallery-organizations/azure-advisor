{
  "info": {
    "name": "Azure Advisor API Get Recommendation",
    "_postman_id": "d1b0ea65-89d7-4c37-972e-1aa6d5fa9453",
    "description": "Retrieves the status of the recommendation computation or generation process. Invoke this API after calling the generation recommendation. The URI of this API is returned in the Location field of the response header.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "recommendations",
      "item": [
        {
          "id": "3d9eeaa1-8c9f-44f1-82e6-3ad53d1c5b63",
          "name": "Recommendations_GetGenerateStatus",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Advisor/generateRecommendations/:operationId"
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
                  "id": "operationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the status of the recommendation computation or generation process"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff5b1b4e-366c-4e39-a2c2-3d6585481bc6"
            }
          ]
        }
      ]
    }
  ]
}