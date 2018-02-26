---
swagger: "2.0"
info:
  title: SchedulerManagementClient
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Scheduler/jobCollections/{jobCollectionName}/jobs/{jobName}
  : get:
      summary: Jobs Get
      description: Gets a job
      operationId: Jobs_Get
      parameters:
      - in: path
        name: jobCollectionName
        description: The job collection name
      - in: path
        name: jobName
        description: The job name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - jobs
definitions:
  JobCollectionListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  JobListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  JobHistoryListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  JobCollectionDefinition:
    properties:
      id:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  JobCollectionProperties:
    properties:
      state:
        description: This is a default description.
        type: get
  Sku:
    properties:
      name:
        description: This is a default description.
        type: get
  JobCollectionQuota:
    properties:
      maxJobCount:
        description: This is a default description.
        type: get
      maxJobOccurrence:
        description: This is a default description.
        type: get
  JobDefinition:
    properties:
      id:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  JobProperties:
    properties:
      startTime:
        description: This is a default description.
        type: get
  JobHistoryDefinition:
    properties:
      id:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  JobHistoryDefinitionProperties:
    properties:
      startTime:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
      expectedExecutionTime:
        description: This is a default description.
        type: get
      actionName:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      retryCount:
        description: This is a default description.
        type: get
      repeatCount:
        description: This is a default description.
        type: get
  JobAction:
    properties:
      type:
        description: This is a default description.
        type: get
  JobErrorAction:
    properties:
      type:
        description: This is a default description.
        type: get
  HttpRequest:
    properties:
      uri:
        description: This is a default description.
        type: get
      method:
        description: This is a default description.
        type: get
      body:
        description: This is a default description.
        type: get
      headers:
        description: This is a default description.
        type: get
  ClientCertAuthentication:
    properties:
      password:
        description: This is a default description.
        type: get
      pfx:
        description: This is a default description.
        type: get
      certificateThumbprint:
        description: This is a default description.
        type: get
      certificateExpirationDate:
        description: This is a default description.
        type: get
      certificateSubjectName:
        description: This is a default description.
        type: get
  BasicAuthentication:
    properties:
      username:
        description: This is a default description.
        type: get
      password:
        description: This is a default description.
        type: get
  OAuthAuthentication:
    properties:
      secret:
        description: This is a default description.
        type: get
      tenant:
        description: This is a default description.
        type: get
      audience:
        description: This is a default description.
        type: get
      clientId:
        description: This is a default description.
        type: get
  HttpAuthentication:
    properties:
      type:
        description: This is a default description.
        type: get
  StorageQueueMessage:
    properties:
      storageAccount:
        description: This is a default description.
        type: get
      queueName:
        description: This is a default description.
        type: get
      sasToken:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  ServiceBusQueueMessage:
    properties:
      queueName:
        description: This is a default description.
        type: get
  ServiceBusTopicMessage:
    properties:
      topicPath:
        description: This is a default description.
        type: get
  ServiceBusMessage:
    properties:
      customMessageProperties:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      namespace:
        description: This is a default description.
        type: get
      transportType:
        description: This is a default description.
        type: get
  ServiceBusAuthentication:
    properties:
      sasKey:
        description: This is a default description.
        type: get
      sasKeyName:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  ServiceBusBrokeredMessageProperties:
    properties:
      contentType:
        description: This is a default description.
        type: get
      correlationId:
        description: This is a default description.
        type: get
      forcePersistence:
        description: This is a default description.
        type: get
      label:
        description: This is a default description.
        type: get
      messageId:
        description: This is a default description.
        type: get
      partitionKey:
        description: This is a default description.
        type: get
      replyTo:
        description: This is a default description.
        type: get
      replyToSessionId:
        description: This is a default description.
        type: get
      scheduledEnqueueTimeUtc:
        description: This is a default description.
        type: get
      sessionId:
        description: This is a default description.
        type: get
  RetryPolicy:
    properties:
      retryType:
        description: This is a default description.
        type: get
      retryInterval:
        description: This is a default description.
        type: get
      retryCount:
        description: This is a default description.
        type: get
  JobMaxRecurrence:
    properties:
      frequency:
        description: This is a default description.
        type: get
      interval:
        description: This is a default description.
        type: get
  JobRecurrence:
    properties:
      frequency:
        description: This is a default description.
        type: get
      interval:
        description: This is a default description.
        type: get
      count:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
  JobRecurrenceSchedule:
    properties:
      weekDays:
        description: This is a default description.
        type: get
      hours:
        description: This is a default description.
        type: get
      minutes:
        description: This is a default description.
        type: get
      monthDays:
        description: This is a default description.
        type: get
      monthlyOccurrences:
        description: This is a default description.
        type: get
  JobRecurrenceScheduleMonthlyOccurrence:
    properties:
      day:
        description: This is a default description.
        type: get
      Occurrence:
        description: This is a default description.
        type: get
  JobStateFilter:
    properties: []
  JobHistoryFilter:
    properties: []
  JobStatus:
    properties:
      executionCount:
        description: This is a default description.
        type: get
      failureCount:
        description: This is a default description.
        type: get
      faultedCount:
        description: This is a default description.
        type: get
      lastExecutionTime:
        description: This is a default description.
        type: get
      nextExecutionTime:
        description: This is a default description.
        type: get
x-collection-name: Azure Scheduler
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