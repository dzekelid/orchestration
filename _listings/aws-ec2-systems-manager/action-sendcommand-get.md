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
  /?Action=SendCommand&k=1:
    get:
      summary: ' Send Command '
      description: Executes commands on one or more remote instances
      operationId: sendCommand
      parameters:
      - in: query
        name: Comment
        description: User-specified information about the command, such as a brief
          description of what the   command should do
        type: string
      - in: query
        name: DocumentHash
        description: The Sha256 or Sha1 hash created by the system when the document
          was created
        type: string
      - in: query
        name: DocumentHashType
        description: Sha256 or Sha1
        type: string
      - in: query
        name: DocumentName
        description: Required
        type: string
      - in: query
        name: InstanceIds
        description: Required
        type: string
      - in: query
        name: MaxConcurrency
        description: (Optional) The maximum number of instances that are allowed to
          execute the command at the   same time
        type: string
      - in: query
        name: MaxErrors
        description: The maximum number of errors allowed without the command failing
        type: string
      - in: query
        name: NotificationConfig
        description: Configurations for sending notifications
        type: string
      - in: query
        name: OutputS3BucketName
        description: The name of the S3 bucket where command execution responses should
          be stored
        type: string
      - in: query
        name: OutputS3KeyPrefix
        description: The directory structure within the S3 bucket where the responses
          should be   stored
        type: string
      - in: query
        name: OutputS3Region
        description: (Optional) The region where the Amazon Simple Storage Service
          (Amazon S3) output bucket is located
        type: string
      - in: query
        name: Parameters
        description: The required and optional parameters specified in the SSM document
          being   executed
        type: string
      - in: query
        name: ServiceRoleArn
        description: The IAM role that Systems Manager uses to send notifications
        type: string
      - in: query
        name: Targets
        description: (Optional) An array of search criteria that targets instances
          using a    Key;Value combination that you specify
        type: string
      - in: query
        name: TimeoutSeconds
        description: If this time is reached and the command has not already started
          executing, it will not   execute
        type: string
      responses:
        200:
          description: OK
      tags:
      - commands
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