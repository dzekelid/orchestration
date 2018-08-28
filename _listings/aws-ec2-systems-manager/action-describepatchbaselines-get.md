---
swagger: "2.0"
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribePatchBaselines&k=1:
    get:
      summary: ' Describe Patch Baselines '
      description: Lists the patch baselines in your AWS account
      operationId: describePatchBaselines
      parameters:
      - in: query
        name: Filters
        description: 'Each element in the array is a structure containing:'
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patch baselines to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - patch baselines
definitions: []
x-collection-name: AWS EC2 Systems Manager
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