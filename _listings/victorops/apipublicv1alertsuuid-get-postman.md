{
  "info": {
    "name": "VictorOps Retrieve alert details.",
    "_postman_id": "2618dc4f-aab3-4fd8-8be4-581c0a3b73eb",
    "description": "Retrieve the details of an alert that was sent VictorOps by you.\n\nThis API may be called a maximum of 6 times per minute.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Continuous Deployment",
      "item": [
        {
          "id": "11d6a7ce-fcc1-4de4-9973-fb3b8722ce0d",
          "name": "api_public.v1.alerts.uuid.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/alerts/:uuid"
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
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the details of an alert that was sent VictorOps by you.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c0696f3-0644-4780-a570-cb6d53f1c931"
            }
          ]
        }
      ]
    }
  ]
}