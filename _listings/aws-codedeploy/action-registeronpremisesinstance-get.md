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
  /?Action=RegisterOnPremisesInstance&k=1:
    get:
      summary: ' Register On Premises Instance '
      description: Registers an on-premises instance
      operationId: registerOnPremisesInstance
      parameters:
      - in: query
        name: iamSessionArn
        description: The ARN of the IAM session to associate with the on-premises
          instance
        type: string
      - in: query
        name: iamUserArn
        description: The ARN of the IAM user to associate with the on-premises instance
        type: string
      - in: query
        name: instanceName
        description: The name of the on-premises instance to register
        type: string
      responses:
        200:
          description: OK
      tags:
      - on premises instances
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