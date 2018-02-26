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
  /?Action=PurgeQueue&k=1:
    get:
      summary: ' Purge Queue '
      description: Deletes the messages in a queue specified by the QueueURL parameter
      operationId: purgeQueue
      parameters:
      - in: query
        name: QueueUrl
        description: The URL of the queue from which the PurgeQueue action deletes
          messages
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