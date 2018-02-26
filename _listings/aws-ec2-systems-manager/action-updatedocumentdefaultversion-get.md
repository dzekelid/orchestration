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
  /?Action=UpdateDocumentDefaultVersion&k=1:
    get:
      summary: ' Update Document Default Version '
      description: Set the default version of a document
      operationId: updateDocumentDefaultVersion
      parameters:
      - in: query
        name: DocumentVersion
        description: The version of a custom document that you want to set as the
          default version
        type: string
      - in: query
        name: Name
        description: The name of a custom document that you want to set as the default
          version
        type: string
      responses:
        200:
          description: OK
      tags:
      - documents
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