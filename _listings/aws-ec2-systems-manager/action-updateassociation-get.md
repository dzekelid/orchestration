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
  /?Action=UpdateAssociation&k=1:
    get:
      summary: ' Update Association '
      description: Updates an association
      operationId: updateAssociation
      parameters:
      - in: query
        name: AssociationId
        description: The ID of the association you want to update
        type: string
      - in: query
        name: DocumentVersion
        description: The document version you want update for the association
        type: string
      - in: query
        name: OutputLocation
        description: An Amazon S3 bucket where you want to store the results of this
          request
        type: string
      - in: query
        name: Parameters
        description: The parameters you want to update for the association
        type: string
      - in: query
        name: ScheduleExpression
        description: The cron expression used to schedule the association that you
          want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - associations
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