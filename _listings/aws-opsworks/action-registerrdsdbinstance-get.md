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
  /?Action=RegisterRdsDbInstance&k=1:
    get:
      summary: ' Register Rds Db Instance '
      description: Registers an Amazon RDS instance with a stack
      operationId: registerRdsDbInstance
      parameters:
      - in: query
        name: DbPassword
        description: The database password
        type: string
      - in: query
        name: DbUser
        description: The database's master user name
        type: string
      - in: query
        name: RdsDbInstanceArn
        description: The Amazon RDS instance's ARN
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - instances
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