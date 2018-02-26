---
swagger: "2.0"
info:
  title: AWS Code Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetThirdPartyJobDetails&k=1:
    get:
      summary: ' Get Third Party Job Details '
      description: Requests the details of a job for a third party action
      operationId: getThirdPartyJobDetails
      parameters:
      - in: query
        name: clientToken
        description: The clientToken portion of the clientId and clientToken pair
          used to verify that            the calling entity is allowed access to the
          job and its details
        type: string
      - in: query
        name: Domain
        description: Set to vpc to allocate the address for use with instances in
          a VPC
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID used for identifying the job
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
definitions: []
x-collection-name: AWS Code Pipeline
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