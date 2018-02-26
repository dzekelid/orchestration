---
swagger: "2.0"
info:
  title: AWS CodeDeploy API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopDeployment&k=1:
    get:
      summary: ' Stop Deployment '
      description: Attempts to stop an ongoing deployment
      operationId: stopDeployment
      parameters:
      - in: query
        name: autoRollbackEnabled
        description: Indicates, when a deployment is stopped, whether instances that
          have been updated            should be rolled back to the previous version
          of the application revision
        type: string
      - in: query
        name: deploymentId
        description: The unique ID of a deployment
        type: string
      responses:
        200:
          description: OK
      tags:
      - deployments
definitions: []
x-collection-name: AWS CodeDeploy
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