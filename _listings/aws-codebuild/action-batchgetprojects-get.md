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
  /?Action=BatchGetProjects&k=1:
    get:
      summary: ' Batch Get Projects '
      description: Gets information about one or more build projects
      operationId: batchGetProjects
      parameters:
      - in: query
        name: names
        description: The names of the build projects to get information about
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