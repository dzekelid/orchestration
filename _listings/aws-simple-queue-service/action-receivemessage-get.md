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
  /?Action=ReceiveMessage&k=1:
    get:
      summary: ' Receive Message '
      description: Retrieves one or more messages (up to 10), from the specified queue
      operationId: receiveMessage
      parameters:
      - in: query
        name: AttributeName.N
        description: A list of attributes that need to be returned along with each
          message
        type: string
      - in: query
        name: MaxNumberOfMessages
        description: The maximum number of messages to return
        type: string
      - in: query
        name: MessageAttributeName.N
        description: The name of the message attribute, where N is the index
        type: string
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue from which messages are received
        type: string
      - in: query
        name: ReceiveRequestAttemptId
        description: This parameter applies only to FIFO (first-in-first-out) queues
        type: string
      - in: query
        name: VisibilityTimeout
        description: The duration (in seconds) that the received messages are hidden
          from subsequent retrieve requests after being retrieved by a ReceiveMessage
          request
        type: string
      - in: query
        name: WaitTimeSeconds
        description: The duration (in seconds) for which the call waits for a message
          to arrive in the queue before returning
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