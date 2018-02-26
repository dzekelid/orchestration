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
  /?Action=DeregisterTaskFromMaintenanceWindow&k=1:
    get:
      summary: ' Deregister Task From Maintenance Window '
      description: Removes a task from a Maintenance Window
      operationId: deregisterTaskFromMaintenanceWindow
      parameters:
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window the task should be removed from
        type: string
      - in: query
        name: WindowTaskId
        description: The ID of the task to remove from the Maintenance Window
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