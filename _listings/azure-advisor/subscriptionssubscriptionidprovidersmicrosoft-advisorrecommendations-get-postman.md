{
  "info": {
    "name": "Azure Advisor API List Recommendations",
    "_postman_id": "fa7f4448-c823-40d4-b07a-eaa55a083963",
    "description": "Obtains cached recommendations for a subscription. The recommendations are generated or computed by invoking generateRecommendations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "recommendations",
      "item": [
        {
          "id": "c7d0870c-9879-4655-a56b-46482375a239",
          "name": "Recommendations_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Advisor/recommendations"
              ],
              "query": [
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$skipToken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains cached recommendations for a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "faf0a54c-d81c-4613-a2cb-370ed8f1941f"
            }
          ]
        }
      ]
    }
  ]
}