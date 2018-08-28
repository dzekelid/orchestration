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
  /?Action=TestRepositoryTriggers&k=1:
    get:
      summary: ' Test Repository Triggers '
      description: Tests the functionality of repository triggers by sending information
        to the trigger target
      operationId: testRepositoryTriggers
      parameters:
      - in: query
        name: repositoryName
        description: The name of the repository in which to test the triggers
        type: string
      - in: query
        name: triggers
        description: The list of triggers to test
        type: string
      responses:
        200:
          description: OK
      tags:
      - repository triggers
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