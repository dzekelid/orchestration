---
swagger: "2.0"
info:
  title: AWS Code Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutApprovalResult&k=1:
    get:
      summary: ' Put Approval Result '
      description: Provides the response to a manual approval request to AWS CodePipeline
      operationId: putApprovalResult
      parameters:
      - in: query
        name: actionName
        description: The name of the action for which approval is requested
        type: string
      - in: query
        name: AllocationId
        description: '[EC2-VPC] The allocation ID'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline that contains the action
        type: string
      - in: query
        name: PublicIp
        description: '[EC2-Classic] The Elastic IP address'
        type: string
      - in: query
        name: result
        description: Represents information about the result of the approval request
        type: string
      - in: query
        name: stageName
        description: The name of the stage that contains the action
        type: string
      - in: query
        name: token
        description: The system-generated token used to identify a unique approval
          request
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
definitions: []
x-collection-name: AWS Code Pipeline
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