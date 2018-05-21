{
  "info": {
    "name": "Azure Advisor API Get Recommendations",
    "_postman_id": "6403d192-6b9f-4050-aaf9-bc461f14674d",
    "description": "Obtains details of a cached recommendation.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "recommendations",
      "item": [
        {
          "id": "5942197c-2bd5-4aa1-81e3-de2dc6cc44ff",
          "name": "Recommendations_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                ":resourceUri/providers/Microsoft.Advisor/recommendations/:recommendationId"
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
                  "id": "recommendationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceUri",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains details of a cached recommendation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "768e9f0e-08bf-4d1a-8e04-7f2c36aecb01"
            }
          ]
        }
      ]
    }
  ]
}