{
  "info": {
    "name": "VictorOps Get a user's on-call schedule",
    "_postman_id": "4beaf2fd-eab0-4d22-9d59-dff22dc093c6",
    "description": "__NOTE: This call is deprecated. Please use `GET /api-public/v2/user/{user}/oncall/schedule`.__\n\nGet the on-call schedule for a user for all teams, including on-call overrides.\n\nThis API may be called a maximum of 15 times per minute.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Continuous Deployment",
      "item": [
        {
          "id": "e0e229af-4b62-47ec-9b8b-ffd343ccb8ca",
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
              "id": "94055d6b-cabd-488e-a012-188f5e599a46"
            }
          ]
        },
        {
          "id": "d83347db-e04b-4a53-990b-4f71587d00cb",
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
              "id": "a5eb8c58-138d-41f1-812c-b9c68a3ca3e2"
            }
          ]
        },
        {
          "id": "bc62ec71-e492-45aa-8a19-e453aa46f92e",
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
              "id": "068910ec-30e4-48b4-838b-4c0d8b2836f9"
            }
          ]
        },
        {
          "id": "b80499d2-b83a-43a7-87ba-f6a8ac399a15",
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
              "id": "069a505c-d5ab-43c6-8017-3ea41ecdb09e"
            }
          ]
        },
        {
          "id": "7cf3ea6b-45c5-41be-b8fc-ef2896962dd0",
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
              "id": "fce844e3-a669-4b68-af08-24bd1ce57a41"
            }
          ]
        },
        {
          "id": "c3e85829-ed2d-4c46-8641-5389f9deb0d1",
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
              "id": "6ac54dbe-e9c0-4e9f-b33b-b781daf826b2"
            }
          ]
        },
        {
          "id": "86205866-fea6-4f4e-9a32-fc957bdf853e",
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
              "id": "0e38c689-b5b9-4f4b-bbfb-8facc96f3012"
            }
          ]
        },
        {
          "id": "8d3ab7fd-86f4-4178-94b0-80d3713b52c1",
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
              "id": "748dfb44-505d-42c4-8493-e8b967b06e35"
            }
          ]
        },
        {
          "id": "53eebf47-64b3-42cf-9300-f84432561b19",
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
              "id": "f3a812cc-e1bc-4a9a-b97a-e233190f8c6c"
            }
          ]
        },
        {
          "id": "12ca99de-b41c-4cc8-aa68-26c6353e179b",
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
              "id": "0d875af1-0d83-42dd-afa4-8874cdb611f8"
            }
          ]
        },
        {
          "id": "8b4ce881-ae00-489f-86f3-b279c08bbef9",
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
              "id": "0aae8e01-6e0b-4269-ae3b-9edfc9f054db"
            }
          ]
        },
        {
          "id": "30f40b53-2fe8-4f8e-9703-144b464d0100",
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
              "id": "97fd9c56-4a18-4bac-8a15-6c78320ab568"
            }
          ]
        },
        {
          "id": "2c7e3a4b-2d3f-49ef-bbb0-ca119c47d413",
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
              "id": "ae408817-d1a5-443c-a03e-5e3129f93309"
            }
          ]
        },
        {
          "id": "65a3c574-ec06-4210-98da-32db1c297b28",
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
              "id": "325f42f3-8bcd-4280-a2bd-3c639bda4488"
            }
          ]
        },
        {
          "id": "fc604935-b3fc-4561-8a22-f72b7664fa7e",
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
              "id": "be7b441a-c561-4b85-8afc-733e6d184641"
            }
          ]
        },
        {
          "id": "eb65313a-79ee-4b72-b1e3-b86e57e87c2a",
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
              "id": "8961558e-2de4-486d-829f-5284b4d872c8"
            }
          ]
        },
        {
          "id": "60c80503-7abb-4bec-aa02-3aa744aa0b5c",
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
              "id": "1132eb24-15cf-4cdb-ab6f-c75aaf92494a"
            }
          ]
        },
        {
          "id": "906d14b8-5a98-45a4-93d4-aab9ef40b5cb",
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
              "id": "2207ed4f-05ac-4310-a949-ddf2b128f8ef"
            }
          ]
        },
        {
          "id": "8de43914-98eb-4ab5-b350-169da2b19ef0",
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
              "id": "849e2b7e-54ed-486e-a20c-98ad1f24df96"
            }
          ]
        },
        {
          "id": "a6e0cac4-773a-4034-a3ae-7abd72b88586",
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
              "id": "f9918c85-43b5-4ed1-bdaf-297e6344dd4d"
            }
          ]
        },
        {
          "id": "15e4c79f-1427-4b98-9702-1cb129d0a4dc",
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
              "id": "7a8e110c-7c5d-4d26-9417-aa8a0d9a97f9"
            }
          ]
        },
        {
          "id": "350b84e7-65ba-4341-a528-69f5e9c4bde5",
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
              "id": "130e08be-d04f-4781-aa24-fa4beae344ce"
            }
          ]
        },
        {
          "id": "ee41533e-4b8e-4d67-bec7-520d1906059d",
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
              "id": "be2037f3-37d1-4be8-ab42-06aefe97eeee"
            }
          ]
        },
        {
          "id": "b30a4ff5-4f6b-45d2-bde0-53f9f7ccae1d",
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
              "id": "51a9a0d5-3508-4f14-b685-5ca853cc51df"
            }
          ]
        },
        {
          "id": "ff9b994a-750f-4dd3-9ee2-398ecef0ce0d",
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
              "id": "19d5d5cf-a041-4999-8e5f-eb593753d163"
            }
          ]
        },
        {
          "id": "c63b0b07-2610-4a82-b967-654c36fd1849",
          "name": "api_public.v1.team.team.get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the information for the specified team.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c362600-533e-4052-ae24-99c6be72534c"
            }
          ]
        },
        {
          "id": "ed253aea-89eb-45da-940e-1029004aeedb",
          "name": "api_public.v1.team.team.put",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update the designated team\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e7da4bf-3217-4e09-b04f-a06ed7bdfe4d"
            }
          ]
        },
        {
          "id": "84c9631c-2bad-4443-b0b6-efb47e596f0c",
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
              "id": "d6711e33-d6f9-4732-be33-25a52e1c09ae"
            }
          ]
        },
        {
          "id": "7f59abfd-9334-490b-a51b-d0347f9a5c6b",
          "name": "api_public.v1.team.team.members.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/members"
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the members for the specified team.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b612a035-f8b1-419f-9562-36d486544d65"
            }
          ]
        },
        {
          "id": "6ca719ce-57df-4773-94b3-63073f1335ad",
          "name": "api_public.v1.team.team.members.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/members"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a team member to your team.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbec7175-fb93-4550-8f9b-091a78f4ed66"
            }
          ]
        },
        {
          "id": "550bdf4b-d8b1-4e9e-bb1e-8ee188fa0a0c",
          "name": "api_public.v1.team.team.members.user.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/members/:user"
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
                },
                {
                  "id": "user",
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
              "id": "91fccdb7-83c9-4cfe-9bb7-c3c07e593dc0"
            }
          ]
        },
        {
          "id": "3c616977-02ff-4c33-8cab-d611a48fc462",
          "name": "api_public.v1.team.team.oncall.schedule.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/oncall/schedule"
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "__NOTE: This call is deprecated. Please use `GET /api-public/v2/team/{team}/oncall/schedule`.__\n\nGet the on-call schedule for a team, including on-call overrides.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9938d14d-00dd-4f44-93fc-3e3e86dec39d"
            }
          ]
        },
        {
          "id": "e1bf9a2c-793f-4338-8836-3e0c640af256",
          "name": "api_public.v1.team.team.oncall.user.patch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/oncall/user"
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
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "__NOTE: This API call is deprecated. Please use `PATCH /api-public/v2/policies/{policy}/oncall/user`__\n\nReplaces a currently on-call user on the team with another.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ad0e11e-30b2-4349-8898-2e3709e19922"
            }
          ]
        },
        {
          "id": "6509c167-a371-413b-928b-cc5769034ddf",
          "name": "api_public.v1.team.team.policies.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/policies"
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the escalation policies for the specified team.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6750af2a-c290-4a18-bc4d-3cdc55d3daff"
            }
          ]
        },
        {
          "id": "ae12ccc6-d495-439d-8ebb-92ead39a6580",
          "name": "api_public.v1.user.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/user?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of users for your organization\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d979473e-03f9-4266-a3f3-2e54632ca717"
            }
          ]
        },
        {
          "id": "0d4dae2e-f2d6-4186-976d-f48149d68167",
          "name": "api_public.v1.user.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/user?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a user to your organization\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d9c3c3c-e1c4-42a5-8381-c13289b3801f"
            }
          ]
        },
        {
          "id": "5126c106-d503-401c-adc2-cd106760247d",
          "name": "api_public.v1.user.user.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the information for the specified user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6638600e-dcea-41e0-b8e3-e4d308da83fb"
            }
          ]
        },
        {
          "id": "ae3fd693-eeff-4a84-91df-d20c4745b4b0",
          "name": "api_public.v1.user.user.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update the designated user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f65321ac-3699-455e-82d1-ad2e8df6d77c"
            }
          ]
        },
        {
          "id": "d1be9882-1a2d-496e-8548-c4ce55e2aa8f",
          "name": "api_public.v1.user.user.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a user from your organization\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcdf08dd-5a90-4ed5-a0c7-f02f813ec33b"
            }
          ]
        },
        {
          "id": "69141f62-7819-49a2-9415-842774fda08f",
          "name": "api_public.v1.user.user.contact_methods.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the contact methods for a user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95de62d5-ef82-42b2-9826-af11e85c4a9d"
            }
          ]
        },
        {
          "id": "90cf8c01-57ce-4fe6-b42e-7532c2134d82",
          "name": "api_public.v1.user.user.contact_methods.devices.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/devices"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the contact methods for a user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "650774e8-bcad-4da2-87eb-d55485e8fb3e"
            }
          ]
        },
        {
          "id": "36b589b4-8f86-44ed-a02f-899ccc30e4a2",
          "name": "api_public.v1.user.user.contact_methods.devices.contactId.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/devices/:contactId"
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
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the indicated contact device for a user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ced06700-e657-413e-8a62-5556cf2dc31d"
            }
          ]
        },
        {
          "id": "7ed3cfa3-ef17-49a0-8466-202a15cc6097",
          "name": "api_public.v1.user.user.contact_methods.devices.contactId.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/devices/:contactId"
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
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a contact device for a user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "727fda13-dd6c-4fb0-afa4-c69dc3535529"
            }
          ]
        },
        {
          "id": "152d05d2-f1d0-4f5e-95cb-4fb9c6dfe2ba",
          "name": "api_public.v1.user.user.contact_methods.devices.contactId.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/devices/:contactId"
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
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a contact device for a user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c112be99-7606-4de7-b3fb-02f481fdeaf8"
            }
          ]
        },
        {
          "id": "0a605db9-2bd8-474e-99c5-d9e9f9511c51",
          "name": "api_public.v1.user.user.contact_methods.emails.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/emails"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the contact emails for a user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20ac9c4c-8764-48d6-8556-df8d327715ac"
            }
          ]
        },
        {
          "id": "dea9f706-ff9d-4d2d-9cca-f44fcf1d42f6",
          "name": "api_public.v1.user.user.contact_methods.emails.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/emails"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a contact email for a user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ee19f53-a1cc-4c8f-9e26-634b718165ec"
            }
          ]
        },
        {
          "id": "b9609502-589f-46a6-927b-b1d92ab8270c",
          "name": "api_public.v1.user.user.contact_methods.emails.contactId.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/emails/:contactId"
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
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the indicated contact email for a user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3676e4e-40a4-4245-9584-c74f0c8d8408"
            }
          ]
        },
        {
          "id": "246e4d02-3b86-4738-8e46-124a6908e1f0",
          "name": "api_public.v1.user.user.contact_methods.emails.contactId.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/emails/:contactId"
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
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the indicated contact email for the user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6211c485-778a-4052-91cb-08d42e09b78e"
            }
          ]
        },
        {
          "id": "797e27e1-a86a-4ce7-be6f-cd4c8595f4be",
          "name": "api_public.v1.user.user.contact_methods.phones.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/phones"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the contact phones for a user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c1b350f-6e8c-4515-bbf8-7677997ff362"
            }
          ]
        },
        {
          "id": "ff3e769b-7d9e-49fe-9915-3e8590a465c2",
          "name": "api_public.v1.user.user.contact_methods.phones.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/phones"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a contact phone for a user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acf6a29d-8d9b-4fa0-8878-e286236c8493"
            }
          ]
        },
        {
          "id": "a57b4a00-c3eb-41e4-9226-f20dc82857f0",
          "name": "api_public.v1.user.user.contact_methods.phones.contactId.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/phones/:contactId"
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
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the indicated contact phone for a user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "102b9b51-fe1a-4ca9-9ae4-9350a0d6a97c"
            }
          ]
        },
        {
          "id": "d605cb9f-4a25-4407-b5fc-5284492aacfa",
          "name": "api_public.v1.user.user.contact_methods.phones.contactId.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/contact-methods/phones/:contactId"
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
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the indicated contact phone for the user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2c18323-653c-4cd3-a19b-772fb2eb6cac"
            }
          ]
        },
        {
          "id": "08fb0cbb-5816-46b0-abce-605fab00c47d",
          "name": "api_public.v1.user.user.oncall.schedule.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user/oncall/schedule"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "__NOTE: This call is deprecated. Please use `GET /api-public/v2/user/{user}/oncall/schedule`.__\n\nGet the on-call schedule for a user for all teams, including on-call overrides.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44c8f012-9d1c-49b6-90b0-6f23a7044dcc"
            }
          ]
        }
      ]
    }
  ]
}