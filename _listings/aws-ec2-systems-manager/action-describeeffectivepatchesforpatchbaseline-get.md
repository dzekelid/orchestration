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
  /?Action=DescribeEffectivePatchesForPatchBaseline&k=1:
    get:
      summary: ' Describe Effective Patches For Patch Baseline '
      description: Retrieves the current effective patches (the patch and the approval
        state) for the specified patch baseline
      operationId: describeEffectivePatchesForPatchBaseline
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to retrieve the effective patches
          for
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patches to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - patches
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