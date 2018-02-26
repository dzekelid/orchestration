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
  /?Action=UpdateManagedInstanceRole&k=1:
    get:
      summary: ' Update Managed Instance Role '
      description: |-
        Assigns or changes an Amazon Identity and Access Management (IAM) role to the managed
           instance
      operationId: updateManagedInstanceRole
      parameters:
      - in: query
        name: IamRole
        description: The IAM role you want to assign or change
        type: string
      - in: query
        name: InstanceId
        description: The ID of the managed instance where you want to update the role
        type: string
      responses:
        200:
          description: OK
      tags:
      - managed instances
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