---
name: Predix
x-slug: predix
description: Predix (IoT PaaS) helps you develop apps that connect people with industrial
  machines through analytics and data for better business outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
x-kinRank: "7"
x-alexaRank: "264121"
tags: Orchestration
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apis.md
specificationVersion: "0.14"
apis:
- name: Analytics Framework - Execute the specified orchestration.
  x-api-slug: apiv1execution-post
  description: To successfully execute the orchestration, the OrchestrationRequest
    must contain valid orchestration id, bpmn workflow xml and optionally input data
    for each analytic step defined in the workflow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv1execution-post-openapi.md
- name: Analytics Framework - Retrieve orchestration execution result
  x-api-slug: apiv1monitoringorchestrationsorchestrationrequestid-get
  description: Returns orchestration execution result for the given orchestration
    request id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv1monitoringorchestrationsorchestrationrequestid-get-openapi.md
- name: Analytics Framework - Get all orchestration configuration entries.
  x-api-slug: apiv2configorchestrations-get
  description: Returns all orchestration configuration entries as specified by page
    and sort criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrations-get-openapi.md
- name: Analytics Framework - Create an orchestration configuration entry.
  x-api-slug: apiv2configorchestrations-post
  description: Creates the orchestration configuration entry with a generated id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrations-post-openapi.md
- name: Analytics Framework - Upload an artifact and attach it to an orchestration
    configuration entry.
  x-api-slug: apiv2configorchestrationsartifacts-post
  description: Upload a single artifact file in a multipart MIME structure and attach
    it to an orchestration configuration entry. The multipart MIME structure must
    have the orchestration entry id tagged as 'orchestrationEntryId',  the file contents
    tagged as 'file',  the artifact type tagged as 'type', and  the name of artifact
    tagged as 'name'.  A description (under 1024 characters) tagged as 'description'
    can be optionally specified. Artifact types can be either 'portToFieldMap', 'bpmn'
    or any.   If the artifact type is 'portToFieldMap', specify the orchestration
    step ID tagged as 'stepId'.   Otherwise, 'name' will be used as 'stepId'.  (See
    the documentation for more information regarding these files.)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsartifacts-post-openapi.md
- name: Analytics Framework - Delete an orchestration artifact by id.
  x-api-slug: apiv2configorchestrationsartifactsid-delete
  description: Delete the orchestration artifact by artifact id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsartifactsid-delete-openapi.md
- name: Analytics Framework - Download an orchestration artifact file by id.
  x-api-slug: apiv2configorchestrationsartifactsidfile-get
  description: The file is downloaded as an octet-stream.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsartifactsidfile-get-openapi.md
- name: Analytics Framework - Get an orchestration configuration entry by id.
  x-api-slug: apiv2configorchestrationsid-get
  description: Returns the orchestration configuration entry with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsid-get-openapi.md
- name: Analytics Framework - Update an existing orchestration configuration entry.
  x-api-slug: apiv2configorchestrationsid-put
  description: Updates the orchestration configuration entry with given orchestration
    configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsid-put-openapi.md
- name: Analytics Framework - Delete an orchestration configuration entry by id.
  x-api-slug: apiv2configorchestrationsid-delete
  description: Deletes the orchestration configuration entry with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsid-delete-openapi.md
- name: Analytics Framework - Get the descriptive information of the orchestration
    artifacts corresponding to an orchestration configuration entry.
  x-api-slug: apiv2configorchestrationsidartifacts-get
  description: 'Returns the description information (type, description, etc.) for
    all orchestration artifacts associated with the given configuration entry id.
    Note: it does not return the orchestration artifact file contents; use the download
    APIs to obtain an artifact file. An error is returned if the supplied orchestration
    configuration entry id does not exist.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsidartifacts-get-openapi.md
- name: Analytics Framework - Download an orchestration artifact file by orchestration
    id and artifact type.
  x-api-slug: apiv2configorchestrationsidfile-get
  description: The file is downloaded as an octet-stream. If the type is bpmn, then
    then bpmn xml is downloaded. If the type is portToFieldMap, then the system expects
    analyticStepId to download the portToFieldMap for the given step
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsidfile-get-openapi.md
- name: Analytics Framework - Execute the specified orchestration.
  x-api-slug: apiv2execution-post
  description: To successfully execute the orchestration, the OrchestrationExecutionRequest
    must contain valid orchestration id, asset id, asset data field mapping details.
    This API will execute the orchestration in synchronous mode and if the execution
    is not completed  in 1 minute then the request will fail. After successful completion,
    the response will contain each orchestration steps output data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2execution-post-openapi.md
- name: Analytics Framework - Execute the specified orchestration in asynchronous
    mode.
  x-api-slug: apiv2executionasync-post
  description: To successfully execute the orchestration, the OrchestrationExecutionRequest
    must contain valid orchestration id, asset id, asset data field mapping details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2executionasync-post-openapi.md
- name: Analytics Framework - Deploy the specified orchestration workflow file to
    the Orchestration Engine.
  x-api-slug: apiv2executionorchestrationsorchconfigiddeployment-post
  description: This API will deploy the BPMN file associated with the specified orchestration
    configuration to the Orchestration Engine in preparation for orchestration execution.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2executionorchestrationsorchconfigiddeployment-post-openapi.md
- name: Analytics Framework - Execute the orchestration with given bpmn and input
    data.
  x-api-slug: apiv2executiontestrun-post
  description: To successfully execute the orchestration, the request must contain
    valid bpmn20.xml, input data for each step in the bpmn.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2executiontestrun-post-openapi.md
- name: Analytics Framework - Validate the specified orchestration and the health
    of all the analytics used in the orchestration.
  x-api-slug: apiv2executionvalidation-post
  description: To successfully validate the orchestration, the BPMN XML file must
    reference analytics that are running. The validation will call a 'healthCheck'
    entry on each analytic.  Analytics in the platform automatically have this entry,
    analytics outside the platform must implement this APIfor their validation to
    pass.  The results contain the http status for each for the healthCheck call to
    each analytic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2executionvalidation-post-openapi.md
- name: Analytics Runtime - Execute the specified orchestration.
  x-api-slug: apiv1execution-post
  description: To successfully execute the orchestration, the OrchestrationRequest
    must contain valid orchestration id, bpmn workflow xml and optionally input data
    for each analytic step defined in the workflow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv1execution-post-openapi.md
- name: Analytics Runtime - Retrieve orchestration execution result
  x-api-slug: apiv1monitoringorchestrationsorchestrationrequestid-get
  description: Returns orchestration execution result for the given orchestration
    request id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv1monitoringorchestrationsorchestrationrequestid-get-openapi.md
- name: Analytics Runtime - Get all orchestration configuration entries.
  x-api-slug: apiv2configorchestrations-get
  description: Returns all orchestration configuration entries as specified by page
    and sort criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrations-get-openapi.md
- name: Analytics Runtime - Create an orchestration configuration entry.
  x-api-slug: apiv2configorchestrations-post
  description: Creates the orchestration configuration entry with a generated id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrations-post-openapi.md
- name: Analytics Runtime - Upload an artifact and attach it to an orchestration configuration
    entry.
  x-api-slug: apiv2configorchestrationsartifacts-post
  description: Upload a single artifact file in a multipart MIME structure and attach
    it to an orchestration configuration entry. The multipart MIME structure must
    have the orchestration entry id tagged as 'orchestrationEntryId',  the file contents
    tagged as 'file',  the artifact type tagged as 'type', and  the name of artifact
    tagged as 'name'.  A description (under 1024 characters) tagged as 'description'
    can be optionally specified. Artifact types can be either 'portToFieldMap', 'bpmn'
    or any.   If the artifact type is 'portToFieldMap', specify the orchestration
    step ID tagged as 'stepId'.   Otherwise, 'name' will be used as 'stepId'.  (See
    the documentation for more information regarding these files.)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsartifacts-post-openapi.md
- name: Analytics Runtime - Delete an orchestration artifact by id.
  x-api-slug: apiv2configorchestrationsartifactsid-delete
  description: Delete the orchestration artifact by artifact id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsartifactsid-delete-openapi.md
- name: Analytics Runtime - Download an orchestration artifact file by id.
  x-api-slug: apiv2configorchestrationsartifactsidfile-get
  description: The file is downloaded as an octet-stream.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsartifactsidfile-get-openapi.md
- name: Analytics Runtime - Get an orchestration configuration entry by id.
  x-api-slug: apiv2configorchestrationsid-get
  description: Returns the orchestration configuration entry with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsid-get-openapi.md
- name: Analytics Runtime - Update an existing orchestration configuration entry.
  x-api-slug: apiv2configorchestrationsid-put
  description: Updates the orchestration configuration entry with given orchestration
    configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsid-put-openapi.md
- name: Analytics Runtime - Delete an orchestration configuration entry by id.
  x-api-slug: apiv2configorchestrationsid-delete
  description: Deletes the orchestration configuration entry with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsid-delete-openapi.md
- name: Analytics Runtime - Get the descriptive information of the orchestration artifacts
    corresponding to an orchestration configuration entry.
  x-api-slug: apiv2configorchestrationsidartifacts-get
  description: 'Returns the description information (type, description, etc.) for
    all orchestration artifacts associated with the given configuration entry id.
    Note: it does not return the orchestration artifact file contents; use the download
    APIs to obtain an artifact file. An error is returned if the supplied orchestration
    configuration entry id does not exist.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsidartifacts-get-openapi.md
- name: Analytics Runtime - Download an orchestration artifact file by orchestration
    id and artifact type.
  x-api-slug: apiv2configorchestrationsidfile-get
  description: The file is downloaded as an octet-stream. If the type is bpmn, then
    then bpmn xml is downloaded. If the type is portToFieldMap, then the system expects
    analyticStepId to download the portToFieldMap for the given step
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2configorchestrationsidfile-get-openapi.md
- name: Analytics Runtime - Execute the specified orchestration.
  x-api-slug: apiv2execution-post
  description: To successfully execute the orchestration, the OrchestrationExecutionRequest
    must contain valid orchestration id, asset id, asset data field mapping details.
    This API will execute the orchestration in synchronous mode and if the execution
    is not completed  in 1 minute then the request will fail. After successful completion,
    the response will contain each orchestration steps output data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2execution-post-openapi.md
- name: Analytics Runtime - Execute the specified orchestration in asynchronous mode.
  x-api-slug: apiv2executionasync-post
  description: To successfully execute the orchestration, the OrchestrationExecutionRequest
    must contain valid orchestration id, asset id, asset data field mapping details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2executionasync-post-openapi.md
- name: Analytics Runtime - Deploy the specified orchestration workflow file to the
    Orchestration Engine.
  x-api-slug: apiv2executionorchestrationsorchconfigiddeployment-post
  description: This API will deploy the BPMN file associated with the specified orchestration
    configuration to the Orchestration Engine in preparation for orchestration execution.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2executionorchestrationsorchconfigiddeployment-post-openapi.md
- name: Analytics Runtime - Execute the orchestration with given bpmn and input data.
  x-api-slug: apiv2executiontestrun-post
  description: To successfully execute the orchestration, the request must contain
    valid bpmn20.xml, input data for each step in the bpmn.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2executiontestrun-post-openapi.md
- name: Analytics Runtime - Validate the specified orchestration and the health of
    all the analytics used in the orchestration.
  x-api-slug: apiv2executionvalidation-post
  description: To successfully validate the orchestration, the BPMN XML file must
    reference analytics that are running. The validation will call a 'healthCheck'
    entry on each analytic.  Analytics in the platform automatically have this entry,
    analytics outside the platform must implement this APIfor their validation to
    pass.  The results contain the http status for each for the healthCheck call to
    each analytic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orchestration/master/_listings/predix/apiv2executionvalidation-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://predicthq.api.gallery.streamdata.io
- type: x-api-stack
  url: http://predix.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/predix
- type: x-documentation
  url: https://docs.predix.io/en-US/platform
- type: x-twitter
  url: https://twitter.com/Predix
- type: x-website
  url: https://www.predix.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---