{
  "info": {
    "name": "VictorOps Remove a team",
    "_postman_id": "9d9edf27-7d66-4de5-a6f1-18e2c5b6cad0",
    "description": "Remove a team from your organization.\n\nThis API may be called a maximum of 15 times per minute.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Continuous Deployment",
      "item": [
        {
          "id": "1b1e26c6-3b78-4632-abc6-a78923064cf2",
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
              "id": "c01d9893-d313-47c9-a9b6-b2ad42ed2789"
            }
          ]
        },
        {
          "id": "f876dc94-b422-4bd1-8f73-5fdc51a82fbe",
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
              "id": "e2cf7260-3edd-48c6-a47e-28e4a2bfa3d5"
            }
          ]
        },
        {
          "id": "ce8ea2a6-33f1-457a-abba-cd52e5b39b7e",
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
              "id": "0862b0a2-2045-463a-b8cb-80d2ff8ede62"
            }
          ]
        },
        {
          "id": "52f689b5-44cb-4c32-afec-d612c072c664",
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
              "id": "1aa4d7d5-bc88-4b84-809f-f3e4324aa445"
            }
          ]
        },
        {
          "id": "f3154da3-1542-46eb-aa54-9a0410053d5d",
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
              "id": "23997deb-912a-4ac9-b5fa-d40e5b9d532c"
            }
          ]
        },
        {
          "id": "1b4eaa62-b11c-49a5-a725-822822f4afe5",
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
              "id": "ae80f7d2-5b16-450b-beb4-fa315f48727d"
            }
          ]
        },
        {
          "id": "eb72a768-8ddf-495f-9319-61ade36a4935",
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
              "id": "1158e950-9026-4d6f-a32c-c03cc1c46e1f"
            }
          ]
        },
        {
          "id": "3c973250-fb4d-44b8-a757-c7906f80d641",
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
              "id": "ec08c273-bcb6-4ae1-a12c-7c110fad41b2"
            }
          ]
        },
        {
          "id": "0f7e5735-777a-4bad-a996-a3a2d129e56c",
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
              "id": "0b415b63-34cd-46e2-a551-07d2dae45128"
            }
          ]
        },
        {
          "id": "6452a364-0ecb-4854-abbe-cf514273886d",
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
              "id": "d57735d5-d098-4ded-92d8-e55c2c724277"
            }
          ]
        },
        {
          "id": "50f5e105-43a6-4333-92a0-ba29b265cf9b",
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
              "id": "9363270e-b531-447e-a09a-1fa4f3bd8040"
            }
          ]
        },
        {
          "id": "c481bc5f-0945-4d03-8ead-82477794f753",
          "name": "api_public.v1.policies.types.contacts.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies/types/contacts?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the available contact types\n\ndescription: \"Email Address\", type: \"email\"\ndescription: \"Phone Number\", type: \"phone\"\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68e787b1-cc25-494a-93b1-ea0d1891a956"
            }
          ]
        },
        {
          "id": "827d8d89-d094-430e-9800-864983f8ce63",
          "name": "api_public.v1.policies.types.notifications.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies/types/notifications?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the available notification types\n\ndescription: \"Send a push notification to all my devices\", type: \"push\"\ndescription: \"Send an email to an email address\", type: \"email\"\ndescription: \"Send an SMS to a phone number\", type: \"sms\"\ndescription: \"Make a phone call to a phone number\", type: \"phone\"\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47d28816-d86e-44e2-aab4-883974117b26"
            }
          ]
        },
        {
          "id": "ee965ee9-c181-4071-b38f-0099d4d5b6ea",
          "name": "api_public.v1.policies.types.timeouts.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies/types/timeouts?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the available timeout values\n\ndescription: \"If still unacked after 1 minute\", type: 1\ndescription: \"If still unacked after 5 minutes\", type: 5\ndescription: \"If still unacked after 10 minutes\", type: 10\ndescription: \"If still unacked after 15 minutes\", type: 15\ndescription: \"If still unacked after 20 minutes\", type: 20\ndescription: \"If still unacked after 25 minutes\", type: 25\ndescription: \"If still unacked after 30 minutes\", type: 30\ndescription: \"If still unacked after 45 minutes\", type: 45\ndescription: \"If still unacked after 60 minutes\", type: 60\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0c8c172-9744-4fec-87f1-2d4d8ae015c1"
            }
          ]
        },
        {
          "id": "3e3af45a-6a26-4c5d-9d02-8f46515e7b74",
          "name": "api_public.v1.policies.policy.oncall.user.patch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/policies/:policy/oncall/user"
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
                  "id": "policy",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Replaces a currently on-call user in the escalation policy with another.  In many cases, the policy slug\nwill match the slug of the team that contains it.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0efd0ca-5371-4266-941e-599b35324e93"
            }
          ]
        },
        {
          "id": "c76dc115-967a-4050-b99f-04d6191059c5",
          "name": "api_public.v1.profile.username.policies.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all the paging policy steps for the user on the org associated with the API key\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e50d7c8-f43c-4015-841f-61b7e3172e07"
            }
          ]
        },
        {
          "id": "a392ff16-99a4-4251-b3b3-e2dd26aa17aa",
          "name": "api_public.v1.profile.username.policies.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e250bd5-7134-4687-a6ef-b0957afb0914"
            }
          ]
        },
        {
          "id": "12eb845b-31dd-4b4d-bfe2-04492d32b752",
          "name": "api_public.v1.profile.username.policies.step.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "912ff5d8-ffdb-401c-836c-a6dd8bff6ed1"
            }
          ]
        },
        {
          "id": "a4f383cf-7ea4-4dcf-b817-258f1bac1699",
          "name": "api_public.v1.profile.username.policies.step.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b200502f-a156-46a1-beb0-486a2e3bf5ad"
            }
          ]
        },
        {
          "id": "9b89ac4c-5054-4a00-a566-114e8af9f734",
          "name": "api_public.v1.profile.username.policies.step.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a rule for a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "493fd70c-3cbd-4314-9390-87f9797027fb"
            }
          ]
        },
        {
          "id": "957c7670-fb90-4099-b8d0-e71001f40035",
          "name": "api_public.v1.profile.username.policies.step.rule.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step/:rule"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                },
                {
                  "id": "rule",
                  "value": "rule",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a rule from a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31743849-94ec-4a24-bf44-d746be4edbba"
            }
          ]
        },
        {
          "id": "40adab3f-9531-4085-acd8-ff7abd569677",
          "name": "api_public.v1.profile.username.policies.step.rule.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step/:rule"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                },
                {
                  "id": "rule",
                  "value": "rule",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a rule for a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e92f31a-cbf2-4627-888d-fd10a40ab963"
            }
          ]
        },
        {
          "id": "2c9e2bc5-f076-4655-8158-759a7df5b36b",
          "name": "api_public.v1.profile.username.policies.step.rule.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step/:rule"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                },
                {
                  "id": "rule",
                  "value": "rule",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a rule from a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "492359d7-6820-42cd-8464-9447ffc215dc"
            }
          ]
        },
        {
          "id": "d7b4a8ca-ccd4-4f53-98f4-1becbb5d51c3",
          "name": "api_public.v1.team.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/team?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of teams for your organization.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "299dfe08-2295-4b23-a326-60327778823c"
            }
          ]
        },
        {
          "id": "671f34c8-b9b9-4e70-920f-f34af6564f41",
          "name": "api_public.v1.team.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/team?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a team to your organization.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9d5c947-6d95-4882-8bfc-10f4884323e7"
            }
          ]
        },
        {
          "id": "1ec4f04f-a929-41a1-af96-fc93a92c250a",
          "name": "api_public.v1.team.team.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team"
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
                  "id": "team",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a team from your organization.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebec7153-1f64-46ef-b17b-f57e1a7afe81"
            }
          ]
        }
      ]
    }
  ]
}