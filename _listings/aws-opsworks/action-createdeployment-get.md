---
swagger: "2.0"
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDeployment&k=1:
    get:
      summary: ' Create Deployment '
      description: Runs deployment or stack commands
      operationId: createDeployment
      parameters:
      - in: query
        name: AppId
        description: The app ID
        type: string
      - in: query
        name: Command
        description: A DeploymentCommand object that specifies the deployment command
          and any      associated arguments
        type: string
      - in: query
        name: Comment
        description: A user-defined comment
        type: string
      - in: query
        name: CustomJson
        description: A string that contains user-defined, custom JSON
        type: string
      - in: query
        name: InstanceIds
        description: The instance IDs for the deployment targets
        type: string
      - in: query
        name: LayerIds
        description: The layer IDs for the deployment targets
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
definitions: []
x-collection-name: AWS OpsWorks
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