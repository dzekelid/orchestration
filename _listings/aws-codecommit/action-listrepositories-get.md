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
  /?Action=ListRepositories&k=1:
    get:
      summary: ' List Repositories '
      description: Gets information about one or more repositories
      operationId: listRepositories
      parameters:
      - in: query
        name: nextToken
        description: An enumeration token that allows the operation to batch the results
          of the operation
        type: string
      - in: query
        name: order
        description: The order in which to sort the results of a list repositories
          operation
        type: string
      - in: query
        name: sortBy
        description: The criteria used to sort the results of a list repositories
          operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - repositories
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