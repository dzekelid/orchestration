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
  /?Action=ListProjects&k=1:
    get:
      summary: ' List Projects '
      description: Gets a list of build project names, with each build project name
        representing a single build project
      operationId: listProjects
      parameters:
      - in: query
        name: nextToken
        description: During a previous call, if there are more than 100 items in the
          list, only the first 100 items are returned, along with a unique string
          called a next token
        type: string
      - in: query
        name: sortBy
        description: The criterion to be used to list build project names
        type: string
      - in: query
        name: sortOrder
        description: The order in which to list build projects
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