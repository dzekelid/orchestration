---
swagger: "2.0"
info:
  title: TaskQueue
  description: Accesses a Google App Engine Pull Task Queue over REST.
  contact:
    name: Google
    url: https://google.com
  version: v1beta2
host: www.googleapis.com
basePath: /taskqueue/v1beta2/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/taskqueues/{taskqueue}:
    get:
      summary: Get Task Queues
      description: Get detailed information about a TaskQueue
      operationId: taskqueue.taskqueues.get
      parameters:
      - in: query
        name: getStats
        description: Whether to get stats
      - in: path
        name: project
        description: The project under which the queue lies
      - in: path
        name: taskqueue
        description: The id of the taskqueue to get the properties of
      responses:
        200:
          description: OK
      tags:
      - task queues
definitions:
  Task:
    properties:
      enqueueTimestamp:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      leaseTimestamp:
        description: This is a default description.
        type: post
      payloadBase64:
        description: This is a default description.
        type: post
      queueName:
        description: This is a default description.
        type: post
      retry_count:
        description: This is a default description.
        type: post
      tag:
        description: This is a default description.
        type: post
  TaskQueue:
    properties:
      acl:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      maxLeases:
        description: This is a default description.
        type: post
      stats:
        description: This is a default description.
        type: post
  Tasks:
    properties:
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  Tasks2:
    properties:
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
x-collection-name: Google Task Queue
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