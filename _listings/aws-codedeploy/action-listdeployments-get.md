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
  /?Action=ListDeployments&k=1:
    get:
      summary: ' List Deployments '
      description: |-
        Lists the deployments in a deployment group for an application registered with the
                    applicable IAM user or AWS account
      operationId: listDeployments
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: createTimeRange
        description: A time range (start and end) for returning a subset of the list
          of            deployments
        type: string
      - in: query
        name: deploymentGroupName
        description: The name of an existing deployment group for the specified application
        type: string
      - in: query
        name: includeOnlyStatuses
        description: 'A subset of deployments to list by status:'
        type: string
      - in: query
        name: nextToken
        description: An identifier returned from the previous list deployments call
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