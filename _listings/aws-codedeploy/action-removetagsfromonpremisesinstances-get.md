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
  /?Action=RemoveTagsFromOnPremisesInstances&k=1:
    get:
      summary: ' Remove Tags From On Premises Instances '
      description: Removes one or more tags from one or more on-premises instances
      operationId: removeTagsFromOnPremisesInstances
      parameters:
      - in: query
        name: instanceNames
        description: The names of the on-premises instances from which to remove tags
        type: string
      - in: query
        name: tags
        description: The tag key-value pairs to remove from the on-premises instances
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