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
  /?Action=ListCommandInvocations&k=1:
    get:
      summary: ' List Command Invocations '
      description: An invocation is copy of a command sent to a specific instance
      operationId: listCommandInvocations
      parameters:
      - in: query
        name: CommandId
        description: (Optional) The invocations for a specific command ID
        type: string
      - in: query
        name: Details
        description: (Optional) If set this returns the response of the command executions
          and any command   output
        type: string
      - in: query
        name: Filters
        description: (Optional) One or more filters
        type: string
      - in: query
        name: InstanceId
        description: (Optional) The command execution details for a specific instance
          ID
        type: string
      - in: query
        name: MaxResults
        description: (Optional) The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: (Optional) The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - command invocations
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