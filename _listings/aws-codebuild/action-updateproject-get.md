---
swagger: "2.0"
info:
  title: AWS CodeBuild API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateProject&k=1:
    get:
      summary: ' Update Project '
      description: Changes the settings of an existing build project
      operationId: updateProject
      parameters:
      - in: query
        name: artifacts
        description: Information to be changed about the build project's build output
          artifacts
        type: string
      - in: query
        name: description
        description: A new or replacement description of the build project
        type: string
      - in: query
        name: encryptionKey
        description: The replacement AWS Key Management Service (AWS KMS) customer
          master key (CMK) to be used for encrypting the build project's build output
          artifacts
        type: string
      - in: query
        name: environment
        description: Information to be changed about the build project's build environment
        type: string
      - in: query
        name: name
        description: The name of the existing build project to change settings
        type: string
      - in: query
        name: serviceRole
        description: The replacement Amazon Resource Name (ARN) of the AWS Identity
          and Access Management (IAM) role that enables AWS CodeBuild to interact
          with dependent AWS services on behalf of the AWS account
        type: string
      - in: query
        name: source
        description: Information to be changed about the build project's build input
          source code
        type: string
      - in: query
        name: tags
        description: The replacement set of tags for this build project
        type: string
      - in: query
        name: timeoutInMinutes
        description: The replacement value in minutes, from 5 to 480 (8 hours), for
          AWS CodeBuild to wait to timeout any related build that did not get marked
          as completed
        type: string
      responses:
        200:
          description: OK
      tags:
      - projects
definitions: []
x-collection-name: AWS CodeBuild
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