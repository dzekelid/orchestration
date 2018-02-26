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
  /?Action=UpdateDocument&k=1:
    get:
      summary: ' Update Document '
      description: The document you want to update
      operationId: updateDocument
      parameters:
      - in: query
        name: Content
        description: The content in a document that you want to update
        type: string
      - in: query
        name: DocumentVersion
        description: The version of the document that you want to update
        type: string
      - in: query
        name: Name
        description: The name of the document that you want to update
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