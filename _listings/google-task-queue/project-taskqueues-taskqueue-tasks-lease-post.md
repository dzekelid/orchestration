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
  /{project}/taskqueues/{taskqueue}/tasks/lease:
    post:
      summary: Lease Task
      description: Lease 1 or more tasks from a TaskQueue
      operationId: taskqueue.tasks.lease
      parameters:
      - in: query
        name: groupByTag
        description: When true, all returned tasks will have the same tag
      - in: query
        name: leaseSecs
        description: The lease in seconds
      - in: query
        name: numTasks
        description: The number of tasks to lease
      - in: path
        name: project
        description: The project under which the queue lies
      - in: query
        name: tag
        description: The tag allowed for tasks in the response
      - in: path
        name: taskqueue
        description: The taskqueue to lease a task from
      responses:
        200:
          description: OK
      tags:
      - task
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