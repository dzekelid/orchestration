---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Runtime Download an orchestration artifact file by orchestration
    id and artifact type.
  version: 1.0.0
  description: The file is downloaded as an octet-stream. If the type is bpmn, then
    then bpmn xml is downloaded. If the type is portToFieldMap, then the system expects
    analyticStepId to download the portToFieldMap for the given step
host: predix-acs.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/execution:
    post:
      summary: Execute the specified orchestration.
      description: To successfully execute the orchestration, the OrchestrationRequest
        must contain valid orchestration id, bpmn workflow xml and optionally input
        data for each analytic step defined in the workflow.
      operationId: run
      x-api-path-slug: apiv1execution-post
      parameters:
      - in: body
        name: body
        description: orchestration execution request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Execute
      - Specified
      - Orchestration
  /api/v1/monitoring/orchestrations/{orchestrationRequestId}:
    get:
      summary: Retrieve orchestration execution result
      description: Returns orchestration execution result for the given orchestration
        request id.
      operationId: retrieveOrchestrationResult
      x-api-path-slug: apiv1monitoringorchestrationsorchestrationrequestid-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: orchestrationRequestId
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Retrieve
      - Orchestration
      - Execution
      - Result
  /api/v2/config/orchestrations:
    get:
      summary: Get all orchestration configuration entries.
      description: Returns all orchestration configuration entries as specified by
        page and sort criteria.
      operationId: retrieveAllOrchConfigs
      x-api-path-slug: apiv2configorchestrations-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: query
        name: page
        description: 'page index : zero-based page index'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: query
        name: size
        description: 'page size : between 1 and 1000 inclusive'
      - in: query
        name: sortableFields
        description: 'sortable fields : name'
      - in: query
        name: sortOrder
        description: 'sort order : asc | desc'
      responses:
        200:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entries
    post:
      summary: Create an orchestration configuration entry.
      description: Creates the orchestration configuration entry with a generated
        id.
      operationId: createOrchestrationEntry
      x-api-path-slug: apiv2configorchestrations-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: orchestration configuration entry
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entry
  /api/v2/config/orchestrations/artifacts:
    post:
      summary: Upload an artifact and attach it to an orchestration configuration
        entry.
      description: Upload a single artifact file in a multipart MIME structure and
        attach it to an orchestration configuration entry. The multipart MIME structure
        must have the orchestration entry id tagged as 'orchestrationEntryId',  the
        file contents tagged as 'file',  the artifact type tagged as 'type', and  the
        name of artifact tagged as 'name'.  A description (under 1024 characters)
        tagged as 'description' can be optionally specified. Artifact types can be
        either 'portToFieldMap', 'bpmn' or any.   If the artifact type is 'portToFieldMap',
        specify the orchestration step ID tagged as 'stepId'.   Otherwise, 'name'
        will be used as 'stepId'.  (See the documentation for more information regarding
        these files.)
      operationId: uploadOrchConfigArtifact
      x-api-path-slug: apiv2configorchestrationsartifacts-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: formData
        name: description
        description: Artifact description
      - in: formData
        name: file
        description: (Required) Artifact file
      - in: formData
        name: name
        description: (Required) Artifact name
      - in: formData
        name: orchestrationEntryId
        description: (Required) orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: formData
        name: stepId
        description: Orchestration Step ID
      - in: formData
        name: type
        description: (Required) Artifact type
      responses:
        200:
          description: Successful response
      tags:
      - Upload
      - Artifact
      - Attach
      - It
      - To
      - Orchestration
      - Configuration
      - Entry
  /api/v2/config/orchestrations/artifacts/{id}:
    delete:
      summary: Delete an orchestration artifact by id.
      description: Delete the orchestration artifact by artifact id.
      operationId: deleteOrchConfigArtifact
      x-api-path-slug: apiv2configorchestrationsartifactsid-delete
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Artifact id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Orchestration
      - Artifact
      - By
      - Id
  /api/v2/config/orchestrations/artifacts/{id}/file:
    get:
      summary: Download an orchestration artifact file by id.
      description: The file is downloaded as an octet-stream.
      operationId: downloadOrchConfigArtifact
      x-api-path-slug: apiv2configorchestrationsartifactsidfile-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Artifact id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Download
      - Orchestration
      - Artifact
      - File
      - By
      - Id
  /api/v2/config/orchestrations/{id}:
    get:
      summary: Get an orchestration configuration entry by id.
      description: Returns the orchestration configuration entry with the given id.
      operationId: retrieveOrchestrationEntryById
      x-api-path-slug: apiv2configorchestrationsid-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entry
      - By
      - Id
    put:
      summary: Update an existing orchestration configuration entry.
      description: Updates the orchestration configuration entry with given orchestration
        configuration.
      operationId: updateOrchestrationEntry
      x-api-path-slug: apiv2configorchestrationsid-put
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: orchestration configuration entry
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: orchestration configuration id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Existing
      - Orchestration
      - Configuration
      - Entry
    delete:
      summary: Delete an orchestration configuration entry by id.
      description: Deletes the orchestration configuration entry with the given id.
      operationId: deleteOrchestrationEntryById
      x-api-path-slug: apiv2configorchestrationsid-delete
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entry
      - By
      - Id
  /api/v2/config/orchestrations/{id}/artifacts:
    get:
      summary: Get the descriptive information of the orchestration artifacts corresponding
        to an orchestration configuration entry.
      description: 'Returns the description information (type, description, etc.)
        for all orchestration artifacts associated with the given configuration entry
        id. Note: it does not return the orchestration artifact file contents; use
        the download APIs to obtain an artifact file. An error is returned if the
        supplied orchestration configuration entry id does not exist.'
      operationId: retrieveArtifactsByOrchestrationEntryId
      x-api-path-slug: apiv2configorchestrationsidartifacts-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Descriptive
      - Information
      - Of
      - Orchestration
      - Artifacts
      - Corresponding
      - To
      - Orchestration
      - Configuration
      - Entry
  /api/v2/config/orchestrations/{id}/file:
    get:
      summary: Download an orchestration artifact file by orchestration id and artifact
        type.
      description: The file is downloaded as an octet-stream. If the type is bpmn,
        then then bpmn xml is downloaded. If the type is portToFieldMap, then the
        system expects analyticStepId to download the portToFieldMap for the given
        step
      operationId: downloadArtifactByType
      x-api-path-slug: apiv2configorchestrationsidfile-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: query
        name: name
        description: artifact name (analytic step id)
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: query
        name: type
        description: artifact type (Ex
      responses:
        200:
          description: Successful response
      tags:
      - Download
      - Orchestration
      - Artifact
      - File
      - By
      - Orchestration
      - Id
      - Artifact
      - Type
  /api/v2/execution:
    post:
      summary: Execute the specified orchestration.
      description: To successfully execute the orchestration, the OrchestrationExecutionRequest
        must contain valid orchestration id, asset id, asset data field mapping details.
        This API will execute the orchestration in synchronous mode and if the execution
        is not completed  in 1 minute then the request will fail. After successful
        completion, the response will contain each orchestration steps output data.
      operationId: runSyncV2
      x-api-path-slug: apiv2execution-post
      parameters:
      - in: body
        name: body
        description: orchestration execution request
        schema:
          $ref: '#/definitions/holder'
      responses:
        2:
          description: Successful response
      tags:
      - Execute
      - Specified
      - Orchestration
  /api/v2/execution/async:
    post:
      summary: Execute the specified orchestration in asynchronous mode.
      description: To successfully execute the orchestration, the OrchestrationExecutionRequest
        must contain valid orchestration id, asset id, asset data field mapping details.
      operationId: runAsync
      x-api-path-slug: apiv2executionasync-post
      parameters:
      - in: body
        name: body
        description: orchestration execution request
        schema:
          $ref: '#/definitions/holder'
      responses:
        2:
          description: Successful response
      tags:
      - Execute
      - Specified
      - Orchestration
      - In
      - Asynchronous
      - Mode
  /api/v2/execution/orchestrations/{orchConfigId}/deployment:
    post:
      summary: Deploy the specified orchestration workflow file to the Orchestration
        Engine.
      description: This API will deploy the BPMN file associated with the specified
        orchestration configuration to the Orchestration Engine in preparation for
        orchestration execution.
      operationId: retrieveAndDeployBpmn
      x-api-path-slug: apiv2executionorchestrationsorchconfigiddeployment-post
      parameters:
      - in: path
        name: orchConfigId
        description: orchestration configuration id
      responses:
        2:
          description: Successful response
      tags:
      - Deploy
      - Specified
      - Orchestration
      - Workflow
      - File
      - To
      - Orchestration
      - Engine
  /api/v2/execution/testrun:
    post:
      summary: Execute the orchestration with given bpmn and input data.
      description: To successfully execute the orchestration, the request must contain
        valid bpmn20.xml, input data for each step in the bpmn.
      operationId: testRun
      x-api-path-slug: apiv2executiontestrun-post
      parameters:
      - in: formData
        name: bpmn
        description: BPMN file
      - in: formData
        name: input
        description: Input data file
      responses:
        2:
          description: Successful response
      tags:
      - Execute
      - Orchestration
      - Given
      - Bpmn
      - Input
      - Data
  /api/v2/execution/validation:
    post:
      summary: Validate the specified orchestration and the health of all the analytics
        used in the orchestration.
      description: To successfully validate the orchestration, the BPMN XML file must
        reference analytics that are running. The validation will call a 'healthCheck'
        entry on each analytic.  Analytics in the platform automatically have this
        entry, analytics outside the platform must implement this APIfor their validation
        to pass.  The results contain the http status for each for the healthCheck
        call to each analytic.
      operationId: validate
      x-api-path-slug: apiv2executionvalidation-post
      parameters:
      - in: body
        name: file
        description: (Required) artifact file
        schema:
          $ref: '#/definitions/holder'
      responses:
        2:
          description: Successful response
      tags:
      - Validate
      - Specified
      - Orchestration
      - Health
      - Of
      - ""
      - Analytics
      - Used
      - In
      - Orchestration
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