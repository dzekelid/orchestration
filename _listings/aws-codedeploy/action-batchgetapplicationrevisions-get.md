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
  /?Action=BatchGetApplicationRevisions&k=1:
    get:
      summary: ' Batch Get Application Revisions '
      description: Gets information about one or more application revisions
      operationId: batchGetApplicationRevisions
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application about which to get
          revision            information
        type: string
      - in: query
        name: revisions
        description: Information to get about the application revisions, including
          type and            location
        type: string
      responses:
        200:
          description: OK
      tags:
      - application revisions
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