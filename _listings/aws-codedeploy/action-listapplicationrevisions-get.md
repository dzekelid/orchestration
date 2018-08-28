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
  /?Action=ListApplicationRevisions&k=1:
    get:
      summary: ' List Application Revisions '
      description: Lists information about revisions for an application
      operationId: listApplicationRevisions
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: deployed
        description: 'Whether to list revisions based on whether the revision is the
          target revision of            an deployment group:'
        type: string
      - in: query
        name: nextToken
        description: An identifier returned from the previous list application revisions
          call
        type: string
      - in: query
        name: s3Bucket
        description: An Amazon S3 bucket name to limit the search for revisions
        type: string
      - in: query
        name: s3KeyPrefix
        description: A key prefix for the set of Amazon S3 objects to limit the search
          for            revisions
        type: string
      - in: query
        name: sortBy
        description: 'The column name to use to sort the list results:'
        type: string
      - in: query
        name: sortOrder
        description: 'The order in which to sort the list results:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - application revisions
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