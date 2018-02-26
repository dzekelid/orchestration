---
swagger: "2.0"
info:
  title: AWS CodeCommit API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListBranches&k=1:
    get:
      summary: ' List Branches '
      description: Gets information about one or more branches in a repository
      operationId: listBranches
      parameters:
      - in: query
        name: nextToken
        description: An enumeration token that allows the operation to batch the results
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository that contains the branches
        type: string
      responses:
        200:
          description: OK
      tags:
      - branches
definitions: []
x-collection-name: AWS CodeCommit
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