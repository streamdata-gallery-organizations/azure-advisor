{
  "info": {
    "name": "Azure Advisor API List Operations",
    "_postman_id": "24e4de3b-a233-4129-b52b-8f7fdde557b8",
    "description": "Lists all the available Advisor REST API operations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "operations",
      "item": [
        {
          "id": "1a1077aa-fa47-46ee-b76c-901bf64b61a9",
          "name": "Operations_List",
          "request": {
            "url": "http://management.azure.com/providers/Microsoft.Advisor/operations?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the available Advisor REST API operations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a37cf92-3bd6-4833-a080-0da145d35131"
            }
          ]
        }
      ]
    }
  ]
}