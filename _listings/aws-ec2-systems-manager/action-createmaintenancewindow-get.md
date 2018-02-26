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
  /?Action=CreateMaintenanceWindow&k=1:
    get:
      summary: ' Create Maintenance Window '
      description: Creates a new Maintenance Window
      operationId: createMaintenanceWindow
      parameters:
      - in: query
        name: AllowUnassociatedTargets
        description: Whether targets must be registered with the Maintenance Window
          before tasks can be   defined for those targets
        type: string
      - in: query
        name: ClientToken
        description: User-provided idempotency token
        type: string
      - in: query
        name: Cutoff
        description: The number of hours before the end of the Maintenance Window
          that Systems Manager stops   scheduling new tasks for execution
        type: string
      - in: query
        name: Duration
        description: The duration of the Maintenance Window in hours
        type: string
      - in: query
        name: Name
        description: The name of the Maintenance Window
        type: string
      - in: query
        name: Schedule
        description: The schedule of the Maintenance Window in the form of a cron
          or rate   expression
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