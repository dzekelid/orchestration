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
  /?Action=UpdateUserProfile&k=1:
    get:
      summary: ' Update User Profile '
      description: Updates a specified user profile
      operationId: updateUserProfile
      parameters:
      - in: query
        name: AllowSelfManagement
        description: Whether users can specify their own SSH public key through the
          My Settings page
        type: string
      - in: query
        name: IamUserArn
        description: The user IAM ARN
        type: string
      - in: query
        name: SshPublicKey
        description: The user's new SSH public key
        type: string
      - in: query
        name: SshUsername
        description: The user's SSH user name
        type: string
      responses:
        200:
          description: OK
      tags:
      - users
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