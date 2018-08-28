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
  /?Action=ChangeMessageVisibility&k=1:
    get:
      summary: ' Change Message Visibility '
      description: Changes the visibility timeout of a specified message in a queue
        to a new value
      operationId: changeMessageVisibility
      parameters:
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue whose message's visibility is
          changed
        type: string
      - in: query
        name: ReceiptHandle
        description: The receipt handle associated with the message whose visibility
          timeout is changed
        type: string
      - in: query
        name: VisibilityTimeout
        description: The new value for the message's visibility timeout (in seconds)
        type: string
      responses:
        200:
          description: OK
      tags:
      - message visibility
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