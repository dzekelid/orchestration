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
  /?Action=PutJobFailureResult&k=1:
    get:
      summary: ' Put Job Failure Result '
      description: Represents the failure of a job as returned to the pipeline by
        a job worker
      operationId: putJobFailureResult
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: failureDetails
        description: The details about the failure of a job
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID of the job that failed
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
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