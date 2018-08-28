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
  /?Action=RegisterTargetWithMaintenanceWindow&k=1:
    get:
      summary: ' Register Target With Maintenance Window '
      description: Registers a target with a Maintenance Window
      operationId: registerTargetWithMaintenanceWindow
      parameters:
      - in: query
        name: ClientToken
        description: User-provided idempotency token
        type: string
      - in: query
        name: OwnerInformation
        description: User-provided value that will be included in any CloudWatch events
          raised while running   tasks for these targets in this Maintenance Window
        type: string
      - in: query
        name: ResourceType
        description: The type of target being registered with the Maintenance Window
        type: string
      - in: query
        name: Targets
        description: The targets (either instances or tags)
        type: string
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window the target should be registered
          with
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