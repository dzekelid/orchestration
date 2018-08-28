{
  "info": {
    "name": "VictorOps Get escalation policy info",
    "_postman_id": "63701a20-8518-4394-a15c-599cf7fc83d4",
    "description": "Retrieves a list of escalation policy information.\nThis API may be called a maximum of once a minute",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Continuous Deployment",
      "item": [
        {
          "id": "a3c29551-05ae-408a-91f0-3f9ee130addf",
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
              "id": "e033bbdb-cd38-4755-9cab-75daa1b73466"
            }
          ]
        },
        {
          "id": "f7c84340-6017-4a54-90c2-aa2d627a8750",
          "name": "api_public.v1.incidents.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of the currently open, acknowledged and recently resolved incidents.\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "822039c9-d63e-47b1-a048-35f89d4c825e"
            }
          ]
        },
        {
          "id": "25a3725c-2563-4b3a-9286-25e8a37585c4",
          "name": "api_public.v1.incidents.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new incident.\n\nThis call replicates the function of our\nmanual incident creation process.\nMonitoring tools and custom integrations\nshould be configured using our\nREST Endpoint.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1ba5b1d-cf70-46a9-b93e-ec83cc4a5984"
            }
          ]
        },
        {
          "id": "e58c139d-311d-45b0-bb02-65277407e618",
          "name": "api_public.v1.incidents.ack.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/ack?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa1e8435-5fcd-4eb6-b9c8-bf0d15c9eaf8"
            }
          ]
        },
        {
          "id": "56966589-2c3f-4187-8809-badbc8417047",
          "name": "api_public.v1.incidents.byUser.ack.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/byUser/ack?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "059c3e46-1c17-40ba-a6ff-ffbb626cfe4b"
            }
          ]
        },
        {
          "id": "d0f99ccd-ab6f-44a1-968b-64e0ec2c3aad",
          "name": "api_public.v1.incidents.byUser.resolve.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/byUser/resolve?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bf22597-a5a4-4cc7-9cb9-44978d9f231a"
            }
          ]
        },
        {
          "id": "d91af00f-3243-4b2f-bc29-0f5164b20746",
          "name": "api_public.v1.incidents.reroute.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/reroute?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reroute one or more incidents to one or more users and/or escalation policies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "422e293f-217d-4297-bcb2-923d2ea145a7"
            }
          ]
        },
        {
          "id": "f5551c55-9715-4de6-9b08-cd503f6b75a6",
          "name": "api_public.v1.incidents.resolve.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/resolve?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5cf73ff-6d3e-4c49-8040-5c98e2b4d424"
            }
          ]
        },
        {
          "id": "df4a05d0-e63a-45e8-b7fc-cf7acc02806c",
          "name": "api_public.v1.oncall.current.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/oncall/current?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all on-call uesrs/teams for your organization.\n\nThis API may be called a maximum of 1 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5727f75e-e6f0-433e-82d8-29e299c81c43"
            }
          ]
        },
        {
          "id": "3c3a46e6-e33f-46b9-99cb-378a03bc8d77",
          "name": "api_public.v1.org.routing_keys.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/org/routing-keys?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of routing keys and associated teams.\nThis API may be called a maximum of once a minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46e80b24-3c9a-4e8e-a1ee-a06c29670967"
            }
          ]
        },
        {
          "id": "17126d5b-1126-4c47-ace5-b49f20ab3599",
          "name": "api_public.v1.policies.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of escalation policy information.\nThis API may be called a maximum of once a minute"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61018abd-8e09-4e48-8e49-4a465e4cecda"
            }
          ]
        }
      ]
    }
  ]
}