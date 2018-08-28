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
  /?Action=ListCuratedEnvironmentImages&k=1:
    get:
      summary: ' List Curated Environment Images '
      description: Gets information about Docker images that are managed by AWS CodeBuild
      operationId: listCuratedEnvironmentImages
      parameters:
      - in: query
        name: platforms
        description: Information about supported platforms for Docker images that
          are managed by AWS CodeBuild
        type: string
      responses:
        200:
          description: OK
      tags:
      - curated environments
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