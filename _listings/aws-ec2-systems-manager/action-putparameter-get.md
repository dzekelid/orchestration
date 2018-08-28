---
swagger: "2.0"
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutParameter&k=1:
    get:
      summary: ' Put Parameter '
      description: Add one or more paramaters to the system
      operationId: putParameter
      parameters:
      - in: query
        name: Description
        description: Information about the parameter that you want to add to the system
        type: string
      - in: query
        name: KeyId
        description: The parameter key ID that you want to add to the system
        type: string
      - in: query
        name: Name
        description: The name of the parameter that you want to add to the system
        type: string
      - in: query
        name: Overwrite
        description: Overwrite an existing parameter
        type: string
      - in: query
        name: Type
        description: The type of parameter that you want to add to the system
        type: string
      - in: query
        name: Value
        description: The parameter value that you want to add to the system
        type: string
      responses:
        200:
          description: OK
      tags:
      - parameters
definitions: []
x-collection-name: AWS EC2 Systems Manager
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---