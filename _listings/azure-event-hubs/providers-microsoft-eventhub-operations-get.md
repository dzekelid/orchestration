---
swagger: "2.0"
info:
  title: EventHubManagementClient
  description: Azure Event Hubs client
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
  /providers/Microsoft.EventHub/operations:
    get:
      summary: Operations List
      description: Lists all of the available Event Hub REST API operations
      operationId: Operations_List
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - operations
definitions:
  OperationListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  Operation:
    properties:
      name:
        description: This is a default description.
        type: get
  TrackedResource:
    properties:
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  Resource:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  NamespaceCreateOrUpdateParameters:
    properties:
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  NamespaceListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  NamespaceResource:
    properties: []
  NamespaceProperties:
    properties:
      status:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
      createdAt:
        description: This is a default description.
        type: get
      updatedAt:
        description: This is a default description.
        type: get
      serviceBusEndpoint:
        description: This is a default description.
        type: get
      metricId:
        description: This is a default description.
        type: get
      enabled:
        description: This is a default description.
        type: get
  Sku:
    properties:
      name:
        description: This is a default description.
        type: get
      tier:
        description: This is a default description.
        type: get
      capacity:
        description: This is a default description.
        type: get
  SharedAccessAuthorizationRuleCreateOrUpdateParameters:
    properties:
      location:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  SharedAccessAuthorizationRuleListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  SharedAccessAuthorizationRuleResource:
    properties: []
  SharedAccessAuthorizationRuleProperties:
    properties:
      rights:
        description: This is a default description.
        type: get
  ResourceListKeys:
    properties:
      primaryConnectionString:
        description: This is a default description.
        type: get
      secondaryConnectionString:
        description: This is a default description.
        type: get
      primaryKey:
        description: This is a default description.
        type: get
      secondaryKey:
        description: This is a default description.
        type: get
      keyName:
        description: This is a default description.
        type: get
  RegenerateKeysParameters:
    properties:
      policykey:
        description: This is a default description.
        type: get
  EventHubCreateOrUpdateParameters:
    properties:
      location:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  EventHubProperties:
    properties:
      createdAt:
        description: This is a default description.
        type: get
      messageRetentionInDays:
        description: This is a default description.
        type: get
      partitionCount:
        description: This is a default description.
        type: get
      partitionIds:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      updatedAt:
        description: This is a default description.
        type: get
  EventHubResource:
    properties: []
  EventHubListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ConsumerGroupCreateOrUpdateParameters:
    properties:
      location:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  ConsumerGroupProperties:
    properties:
      createdAt:
        description: This is a default description.
        type: get
      eventHubPath:
        description: This is a default description.
        type: get
      updatedAt:
        description: This is a default description.
        type: get
      userMetadata:
        description: This is a default description.
        type: get
  ConsumerGroupResource:
    properties: []
  ConsumerGroupListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  CheckNameAvailabilityParameter:
    properties:
      name:
        description: This is a default description.
        type: get
  CheckNameAvailabilityResult:
    properties:
      nameAvailable:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  NamespaceUpdateParameter:
    properties:
      tags:
        description: This is a default description.
        type: get
x-collection-name: Azure Event Hubs
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