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
  /?Action=ListOnPremisesInstances&k=1:
    get:
      summary: ' List On Premises Instances '
      description: Gets a list of names for one or more on-premises instances
      operationId: listOnPremisesInstances
      parameters:
      - in: query
        name: nextToken
        description: An identifier returned from the previous list on-premises instances
          call
        type: string
      - in: query
        name: registrationStatus
        description: 'The registration status of the on-premises instances:'
        type: string
      - in: query
        name: tagFilters
        description: The on-premises instance tags that will be used to restrict the
          corresponding            on-premises instance names returned
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