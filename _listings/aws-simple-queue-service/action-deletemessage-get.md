---
swagger: "2.0"
info:
  title: AWS Simple Queue Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteMessage&k=1:
    get:
      summary: ' Delete Message '
      description: Deletes the specified message from the specified queue
      operationId: deleteMessage
      parameters:
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue from which messages are deleted
        type: string
      - in: query
        name: ReceiptHandle
        description: The receipt handle associated with the message to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - messages
definitions: []
x-collection-name: AWS Simple Queue Service
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