---
swagger: "2.0"
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeUserProfiles&k=1:
    get:
      summary: ' Describe User Profiles '
      description: Describe specified users
      operationId: describeUserProfiles
      parameters:
      - in: query
        name: IamUserArns
        description: An array of IAM or federated user ARNs that identify the users
          to be described
        type: string
      responses:
        200:
          description: OK
      tags:
      - users
definitions: []
x-collection-name: AWS OpsWorks
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