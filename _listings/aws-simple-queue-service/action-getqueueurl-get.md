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
  /?Action=GetQueueUrl&k=1:
    get:
      summary: ' Get Queue Url '
      description: Returns the URL of an existing queue
      operationId: getQueueUrl
      parameters:
      - in: query
        name: QueueName
        description: The name of the queue whose URL must be fetched
        type: string
      - in: query
        name: QueueOwnerAWSAccountId
        description: The AWS account ID of the account that created the queue
        type: string
      responses:
        200:
          description: OK
      tags:
      - queues
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