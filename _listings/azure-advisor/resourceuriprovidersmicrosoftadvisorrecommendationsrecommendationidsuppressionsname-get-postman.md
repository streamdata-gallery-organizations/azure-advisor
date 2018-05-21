{
  "info": {
    "name": "Azure Advisor API Get Suppressions",
    "_postman_id": "9a855135-7fc9-4dfb-b16a-3e3fc8704b4f",
    "description": "Obtains the details of a suppression.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Recommendations",
      "item": [
        {
          "id": "6c59c15b-a758-4b38-9f58-97f4efd6691d",
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
            "description": "Initiates the recommendation generation or computation process for a subscription. This operation is asynchronous. The generated recommendations are stored in a cache in the Advisor service."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43669aa6-1a01-4cf4-9d46-f043bfdf91a1"
            }
          ]
        },
        {
          "id": "20722034-e13b-47b5-a645-a17d906024c7",
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
            "description": "Retrieves the status of the recommendation computation or generation process. Invoke this API after calling the generation recommendation. The URI of this API is returned in the Location field of the response header."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4920875-f904-4989-8b52-191e7bc93e2b"
            }
          ]
        },
        {
          "id": "6d23dcc5-3e05-4177-8223-6f4e820e4152",
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
            "description": "Obtains cached recommendations for a subscription. The recommendations are generated or computed by invoking generateRecommendations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b3435db-7146-4cf9-87b4-9c5e3b31d304"
            }
          ]
        }
      ]
    },
    {
      "name": "Operations",
      "item": [
        {
          "id": "defcd3f3-d9e9-4a54-bb6c-2940dc9d8ac8",
          "name": "Operations_List",
          "request": {
            "url": "http://management.azure.com/providers/Microsoft.Advisor/operations?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the available Advisor REST API operations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c257b843-e595-4d0e-89de-00a8d5b5010e"
            }
          ]
        }
      ]
    },
    {
      "name": "Suppressions",
      "item": [
        {
          "id": "8394576b-55e8-4097-b147-640ae218b3e3",
          "name": "Suppressions_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                ":resourceUri/providers/Microsoft.Advisor/recommendations/:recommendationId/suppressions/:name"
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
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Obtains the details of a suppression."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b408a933-2961-4a1a-80e7-fb7b05cbb765"
            }
          ]
        }
      ]
    }
  ]
}