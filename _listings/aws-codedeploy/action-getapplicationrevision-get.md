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
  /?Action=GetApplicationRevision&k=1:
    get:
      summary: ' Get Application Revision '
      description: Gets information about an application revision
      operationId: getApplicationRevision
      parameters:
      - in: query
        name: applicationName
        description: The name of the application that corresponds to the revision
        type: string
      - in: query
        name: revision
        description: Information about the application revision to get, including
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