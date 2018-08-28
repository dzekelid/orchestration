---
swagger: "2.0"
info:
  title: AWS Step Functions API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteStateMachine&k=1:
    get:
      summary: ' Delete State Machine '
      description: Deletes a state machine
      operationId: deleteStateMachine
      parameters:
      - in: query
        name: stateMachineArn
        description: The Amazon Resource Name (ARN) of the state machine to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - state machine
definitions: []
x-collection-name: AWS Step Functions
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