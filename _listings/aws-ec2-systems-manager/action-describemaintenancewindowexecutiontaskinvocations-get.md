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
  /?Action=DescribeMaintenanceWindowExecutionTaskInvocations&k=1:
    get:
      summary: ' Describe Maintenance Window Execution Task Invocations '
      description: |-
        Retrieves the individual task executions (one per target) for a particular task executed
           as part of a Maintenance Window execution
      operationId: describeMaintenanceWindowExecutionTaskInvocations
      parameters:
      - in: query
        name: Filters
        description: Optional filters used to scope down the returned task invocations
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: TaskId
        description: The ID of the specific task in the Maintenance Window task that
          should be   retrieved
        type: string
      - in: query
        name: WindowExecutionId
        description: The ID of the Maintenance Window execution the task is part of
        type: string
      responses:
        200:
          description: OK
      tags:
      - maintenance windows
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