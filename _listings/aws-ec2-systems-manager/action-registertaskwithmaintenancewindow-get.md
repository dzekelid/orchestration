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
  /?Action=RegisterTaskWithMaintenanceWindow&k=1:
    get:
      summary: ' Register Task With Maintenance Window '
      description: Adds a new task to a Maintenance Window
      operationId: registerTaskWithMaintenanceWindow
      parameters:
      - in: query
        name: ClientToken
        description: User-provided idempotency token
        type: string
      - in: query
        name: LoggingInfo
        description: A structure containing information about an Amazon S3 bucket
          to write instance-level logs to
        type: string
      - in: query
        name: MaxConcurrency
        description: The maximum number of targets this task can be run for in parallel
        type: string
      - in: query
        name: MaxErrors
        description: The maximum number of errors allowed before this task stops being
          scheduled
        type: string
      - in: query
        name: Priority
        description: The priority of the task in the Maintenance Window, the lower
          the number the higher the   priority
        type: string
      - in: query
        name: ServiceRoleArn
        description: The role that should be assumed when executing the task
        type: string
      - in: query
        name: Targets
        description: The targets (either instances or tags)
        type: string
      - in: query
        name: TaskArn
        description: The ARN of the task to execute
        type: string
      - in: query
        name: TaskParameters
        description: The parameters that should be passed to the task when it is executed
        type: string
      - in: query
        name: TaskType
        description: The type of task being registered
        type: string
      - in: query
        name: WindowId
        description: The id of the Maintenance Window the task should be added to
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