---
swagger: "2.0"
info:
  title: Google Dataflow
  description: Manages Google Cloud Dataflow projects on Google Cloud Platform.
  contact:
    name: Google
    url: https://google.com
  version: v1b3
host: dataflow.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1b3/projects/{projectId}/jobs/{jobId}:
    get:
      summary: Get Project Job
      description: Gets the state of the specified Cloud Dataflow job
      operationId: dataflow.projects.jobs.get
      parameters:
      - in: path
        name: jobId
        description: The job ID
      - in: query
        name: location
        description: The location that contains this job
      - in: path
        name: projectId
        description: The ID of the Cloud Platform project that the job belongs to
      - in: query
        name: view
        description: The level of information requested in response
      responses:
        200:
          description: OK
      tags:
      - job
definitions:
  ApproximateProgress:
    properties:
      percentComplete:
        description: This is a default description.
        type: post
      remainingTime:
        description: This is a default description.
        type: post
  ApproximateReportedProgress:
    properties:
      fractionConsumed:
        description: This is a default description.
        type: post
  ApproximateSplitRequest:
    properties:
      fractionConsumed:
        description: This is a default description.
        type: post
  AutoscalingSettings:
    properties:
      algorithm:
        description: This is a default description.
        type: post
      maxNumWorkers:
        description: This is a default description.
        type: post
  CPUTime:
    properties:
      rate:
        description: This is a default description.
        type: post
      timestamp:
        description: This is a default description.
        type: post
      totalMs:
        description: This is a default description.
        type: post
  ComponentSource:
    properties:
      name:
        description: This is a default description.
        type: post
      originalTransformOrCollection:
        description: This is a default description.
        type: post
      userName:
        description: This is a default description.
        type: post
  ComponentTransform:
    properties:
      name:
        description: This is a default description.
        type: post
      originalTransform:
        description: This is a default description.
        type: post
      userName:
        description: This is a default description.
        type: post
  ComputationTopology:
    properties:
      computationId:
        description: This is a default description.
        type: post
      inputs:
        description: This is a default description.
        type: post
      keyRanges:
        description: This is a default description.
        type: post
      outputs:
        description: This is a default description.
        type: post
      stateFamilies:
        description: This is a default description.
        type: post
      systemStageName:
        description: This is a default description.
        type: post
      userStageName:
        description: This is a default description.
        type: post
  ConcatPosition:
    properties:
      index:
        description: This is a default description.
        type: post
  CounterMetadata:
    properties:
      description:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      otherUnits:
        description: This is a default description.
        type: post
      standardUnits:
        description: This is a default description.
        type: post
  CounterStructuredName:
    properties:
      componentStepName:
        description: This is a default description.
        type: post
      executionStepName:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      origin:
        description: This is a default description.
        type: post
      originNamespace:
        description: This is a default description.
        type: post
      originalStepName:
        description: This is a default description.
        type: post
      portion:
        description: This is a default description.
        type: post
      workerId:
        description: This is a default description.
        type: post
  CounterStructuredNameAndMetadata:
    properties: []
  CounterUpdate:
    properties:
      boolean:
        description: This is a default description.
        type: post
      cumulative:
        description: This is a default description.
        type: post
      floatingPoint:
        description: This is a default description.
        type: post
      shortId:
        description: This is a default description.
        type: post
  CreateJobFromTemplateRequest:
    properties:
      gcsPath:
        description: This is a default description.
        type: post
      jobName:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
  CustomSourceLocation:
    properties:
      stateful:
        description: This is a default description.
        type: post
  DataDiskAssignment:
    properties:
      dataDisks:
        description: This is a default description.
        type: post
      vmInstance:
        description: This is a default description.
        type: post
  DerivedSource:
    properties:
      derivationMode:
        description: This is a default description.
        type: post
  Disk:
    properties:
      diskType:
        description: This is a default description.
        type: post
      mountPoint:
        description: This is a default description.
        type: post
      sizeGb:
        description: This is a default description.
        type: post
  DisplayData:
    properties:
      boolValue:
        description: This is a default description.
        type: post
      durationValue:
        description: This is a default description.
        type: post
      floatValue:
        description: This is a default description.
        type: post
      int64Value:
        description: This is a default description.
        type: post
      javaClassValue:
        description: This is a default description.
        type: post
      key:
        description: This is a default description.
        type: post
      label:
        description: This is a default description.
        type: post
      namespace:
        description: This is a default description.
        type: post
      shortStrValue:
        description: This is a default description.
        type: post
      strValue:
        description: This is a default description.
        type: post
  DistributionUpdate:
    properties:
      sumOfSquares:
        description: This is a default description.
        type: post
  DynamicSourceSplit:
    properties: []
  Environment:
    properties:
      clusterManagerApiService:
        description: This is a default description.
        type: post
      dataset:
        description: This is a default description.
        type: post
      experiments:
        description: This is a default description.
        type: post
      internalExperiments:
        description: This is a default description.
        type: post
      sdkPipelineOptions:
        description: This is a default description.
        type: post
      serviceAccountEmail:
        description: This is a default description.
        type: post
      tempStoragePrefix:
        description: This is a default description.
        type: post
      userAgent:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
      workerPools:
        description: This is a default description.
        type: post
  ExecutionStageSummary:
    properties:
      componentSource:
        description: This is a default description.
        type: post
      componentTransform:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      inputSource:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      outputSource:
        description: This is a default description.
        type: post
  FailedLocation:
    properties:
      name:
        description: This is a default description.
        type: post
  FlattenInstruction:
    properties:
      inputs:
        description: This is a default description.
        type: post
  FloatingPointList:
    properties:
      elements:
        description: This is a default description.
        type: post
  FloatingPointMean:
    properties:
      sum:
        description: This is a default description.
        type: post
  GetDebugConfigRequest:
    properties:
      componentId:
        description: This is a default description.
        type: post
      workerId:
        description: This is a default description.
        type: post
  GetDebugConfigResponse:
    properties:
      config:
        description: This is a default description.
        type: post
  GetTemplateResponse:
    properties: []
  InstructionInput:
    properties:
      outputNum:
        description: This is a default description.
        type: post
      producerInstructionIndex:
        description: This is a default description.
        type: post
  InstructionOutput:
    properties:
      codec:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      onlyCountKeyBytes:
        description: This is a default description.
        type: post
      onlyCountValueBytes:
        description: This is a default description.
        type: post
      originalName:
        description: This is a default description.
        type: post
      systemName:
        description: This is a default description.
        type: post
  IntegerList:
    properties:
      elements:
        description: This is a default description.
        type: post
  IntegerMean:
    properties: []
  Job:
    properties:
      clientRequestId:
        description: This is a default description.
        type: post
      createTime:
        description: This is a default description.
        type: post
      currentState:
        description: This is a default description.
        type: post
      currentStateTime:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      labels:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      projectId:
        description: This is a default description.
        type: post
      replaceJobId:
        description: This is a default description.
        type: post
  JobExecutionInfo:
    properties:
      stages:
        description: This is a default description.
        type: post
  JobExecutionStageInfo:
    properties:
      stepName:
        description: This is a default description.
        type: post
  JobMessage:
    properties:
      id:
        description: This is a default description.
        type: post
      messageImportance:
        description: This is a default description.
        type: post
      messageText:
        description: This is a default description.
        type: post
      time:
        description: This is a default description.
        type: post
  JobMetrics:
    properties:
      metricTime:
        description: This is a default description.
        type: post
      metrics:
        description: This is a default description.
        type: post
  KeyRangeDataDiskAssignment:
    properties:
      dataDisk:
        description: This is a default description.
        type: post
      end:
        description: This is a default description.
        type: post
      start:
        description: This is a default description.
        type: post
  KeyRangeLocation:
    properties:
      dataDisk:
        description: This is a default description.
        type: post
      deliveryEndpoint:
        description: This is a default description.
        type: post
      end:
        description: This is a default description.
        type: post
      persistentDirectory:
        description: This is a default description.
        type: post
      start:
        description: This is a default description.
        type: post
  LaunchTemplateParameters:
    properties:
      jobName:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
  LaunchTemplateResponse:
    properties: []
  LeaseWorkItemRequest:
    properties:
      currentWorkerTime:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      requestedLeaseDuration:
        description: This is a default description.
        type: post
      workItemTypes:
        description: This is a default description.
        type: post
      workerCapabilities:
        description: This is a default description.
        type: post
      workerId:
        description: This is a default description.
        type: post
  LeaseWorkItemResponse:
    properties:
      workItems:
        description: This is a default description.
        type: post
  ListJobMessagesResponse:
    properties:
      jobMessages:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
  ListJobsResponse:
    properties:
      failedLocation:
        description: This is a default description.
        type: post
      jobs:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
  MapTask:
    properties:
      instructions:
        description: This is a default description.
        type: post
      stageName:
        description: This is a default description.
        type: post
      systemName:
        description: This is a default description.
        type: post
  MetricShortId:
    properties:
      metricIndex:
        description: This is a default description.
        type: post
      shortId:
        description: This is a default description.
        type: post
  MetricStructuredName:
    properties:
      context:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      origin:
        description: This is a default description.
        type: post
  MetricUpdate:
    properties:
      cumulative:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      updateTime:
        description: This is a default description.
        type: post
  MountedDataDisk:
    properties:
      dataDisk:
        description: This is a default description.
        type: post
  MultiOutputInfo:
    properties:
      tag:
        description: This is a default description.
        type: post
  NameAndKind:
    properties:
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  Package:
    properties:
      location:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  ParDoInstruction:
    properties:
      multiOutputInfos:
        description: This is a default description.
        type: post
      numOutputs:
        description: This is a default description.
        type: post
      sideInputs:
        description: This is a default description.
        type: post
      userFn:
        description: This is a default description.
        type: post
  ParallelInstruction:
    properties:
      name:
        description: This is a default description.
        type: post
      originalName:
        description: This is a default description.
        type: post
      outputs:
        description: This is a default description.
        type: post
      systemName:
        description: This is a default description.
        type: post
  ParameterMetadata:
    properties:
      helpText:
        description: This is a default description.
        type: post
      isOptional:
        description: This is a default description.
        type: post
      label:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      regexes:
        description: This is a default description.
        type: post
  PartialGroupByKeyInstruction:
    properties:
      inputElementCodec:
        description: This is a default description.
        type: post
      originalCombineValuesInputStoreName:
        description: This is a default description.
        type: post
      originalCombineValuesStepName:
        description: This is a default description.
        type: post
      sideInputs:
        description: This is a default description.
        type: post
      valueCombiningFn:
        description: This is a default description.
        type: post
  PipelineDescription:
    properties:
      displayData:
        description: This is a default description.
        type: post
      executionPipelineStage:
        description: This is a default description.
        type: post
      originalPipelineTransform:
        description: This is a default description.
        type: post
  Position:
    properties:
      byteOffset:
        description: This is a default description.
        type: post
      end:
        description: This is a default description.
        type: post
      key:
        description: This is a default description.
        type: post
      recordIndex:
        description: This is a default description.
        type: post
      shufflePosition:
        description: This is a default description.
        type: post
  PubsubLocation:
    properties:
      dropLateData:
        description: This is a default description.
        type: post
      idLabel:
        description: This is a default description.
        type: post
      subscription:
        description: This is a default description.
        type: post
      timestampLabel:
        description: This is a default description.
        type: post
      topic:
        description: This is a default description.
        type: post
      trackingSubscription:
        description: This is a default description.
        type: post
      withAttributes:
        description: This is a default description.
        type: post
  ReadInstruction:
    properties: []
  ReportWorkItemStatusRequest:
    properties:
      currentWorkerTime:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      workItemStatuses:
        description: This is a default description.
        type: post
      workerId:
        description: This is a default description.
        type: post
  ReportWorkItemStatusResponse:
    properties:
      workItemServiceStates:
        description: This is a default description.
        type: post
  ReportedParallelism:
    properties:
      isInfinite:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  ResourceUtilizationReport:
    properties:
      cpuTime:
        description: This is a default description.
        type: post
  ResourceUtilizationReportResponse:
    properties: []
  RuntimeEnvironment:
    properties:
      bypassTempDirValidation:
        description: This is a default description.
        type: post
      maxWorkers:
        description: This is a default description.
        type: post
      serviceAccountEmail:
        description: This is a default description.
        type: post
      tempLocation:
        description: This is a default description.
        type: post
      zone:
        description: This is a default description.
        type: post
  SendDebugCaptureRequest:
    properties:
      componentId:
        description: This is a default description.
        type: post
      data:
        description: This is a default description.
        type: post
      workerId:
        description: This is a default description.
        type: post
  SendDebugCaptureResponse:
    properties: []
  SendWorkerMessagesRequest:
    properties:
      workerMessages:
        description: This is a default description.
        type: post
  SendWorkerMessagesResponse:
    properties:
      workerMessageResponses:
        description: This is a default description.
        type: post
  SeqMapTask:
    properties:
      inputs:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      outputInfos:
        description: This is a default description.
        type: post
      stageName:
        description: This is a default description.
        type: post
      systemName:
        description: This is a default description.
        type: post
      userFn:
        description: This is a default description.
        type: post
  SeqMapTaskOutputInfo:
    properties:
      tag:
        description: This is a default description.
        type: post
  ShellTask:
    properties:
      command:
        description: This is a default description.
        type: post
      exitCode:
        description: This is a default description.
        type: post
  SideInputInfo:
    properties:
      kind:
        description: This is a default description.
        type: post
      sources:
        description: This is a default description.
        type: post
      tag:
        description: This is a default description.
        type: post
  Sink:
    properties:
      codec:
        description: This is a default description.
        type: post
      spec:
        description: This is a default description.
        type: post
  Source:
    properties:
      baseSpecs:
        description: This is a default description.
        type: post
      codec:
        description: This is a default description.
        type: post
      doesNotNeedSplitting:
        description: This is a default description.
        type: post
      spec:
        description: This is a default description.
        type: post
  SourceFork:
    properties: []
  SourceGetMetadataRequest:
    properties: []
  SourceGetMetadataResponse:
    properties: []
  SourceMetadata:
    properties:
      estimatedSizeBytes:
        description: This is a default description.
        type: post
      infinite:
        description: This is a default description.
        type: post
      producesSortedKeys:
        description: This is a default description.
        type: post
  SourceOperationRequest:
    properties: []
  SourceOperationResponse:
    properties: []
  SourceSplitOptions:
    properties:
      desiredBundleSizeBytes:
        description: This is a default description.
        type: post
      desiredShardSizeBytes:
        description: This is a default description.
        type: post
  SourceSplitRequest:
    properties: []
  SourceSplitResponse:
    properties:
      bundles:
        description: This is a default description.
        type: post
      outcome:
        description: This is a default description.
        type: post
      shards:
        description: This is a default description.
        type: post
  SourceSplitShard:
    properties:
      derivationMode:
        description: This is a default description.
        type: post
  SplitInt64:
    properties:
      highBits:
        description: This is a default description.
        type: post
      lowBits:
        description: This is a default description.
        type: post
  StageSource:
    properties:
      name:
        description: This is a default description.
        type: post
      originalTransformOrCollection:
        description: This is a default description.
        type: post
      sizeBytes:
        description: This is a default description.
        type: post
      userName:
        description: This is a default description.
        type: post
  StateFamilyConfig:
    properties:
      isRead:
        description: This is a default description.
        type: post
      stateFamily:
        description: This is a default description.
        type: post
  Status:
    properties:
      code:
        description: This is a default description.
        type: post
      details:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  Step:
    properties:
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      properties:
        description: This is a default description.
        type: post
  StreamLocation:
    properties: []
  StreamingComputationConfig:
    properties:
      computationId:
        description: This is a default description.
        type: post
      instructions:
        description: This is a default description.
        type: post
      stageName:
        description: This is a default description.
        type: post
      systemName:
        description: This is a default description.
        type: post
  StreamingComputationRanges:
    properties:
      computationId:
        description: This is a default description.
        type: post
      rangeAssignments:
        description: This is a default description.
        type: post
  StreamingComputationTask:
    properties:
      computationRanges:
        description: This is a default description.
        type: post
      dataDisks:
        description: This is a default description.
        type: post
      taskType:
        description: This is a default description.
        type: post
  StreamingConfigTask:
    properties:
      streamingComputationConfigs:
        description: This is a default description.
        type: post
      userStepToStateFamilyNameMap:
        description: This is a default description.
        type: post
  StreamingSetupTask:
    properties:
      drain:
        description: This is a default description.
        type: post
      receiveWorkPort:
        description: This is a default description.
        type: post
      workerHarnessPort:
        description: This is a default description.
        type: post
  StreamingSideInputLocation:
    properties:
      stateFamily:
        description: This is a default description.
        type: post
      tag:
        description: This is a default description.
        type: post
  StreamingStageLocation:
    properties:
      streamId:
        description: This is a default description.
        type: post
  StringList:
    properties:
      elements:
        description: This is a default description.
        type: post
  TaskRunnerSettings:
    properties:
      alsologtostderr:
        description: This is a default description.
        type: post
      baseTaskDir:
        description: This is a default description.
        type: post
      baseUrl:
        description: This is a default description.
        type: post
      commandlinesFileName:
        description: This is a default description.
        type: post
      continueOnException:
        description: This is a default description.
        type: post
      dataflowApiVersion:
        description: This is a default description.
        type: post
      harnessCommand:
        description: This is a default description.
        type: post
      languageHint:
        description: This is a default description.
        type: post
      logDir:
        description: This is a default description.
        type: post
      logToSerialconsole:
        description: This is a default description.
        type: post
  TemplateMetadata:
    properties:
      bypassTempDirValidation:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
  TopologyConfig:
    properties:
      computations:
        description: This is a default description.
        type: post
      dataDiskAssignments:
        description: This is a default description.
        type: post
      forwardingKeyBits:
        description: This is a default description.
        type: post
      persistentStateVersion:
        description: This is a default description.
        type: post
      userStageToComputationNameMap:
        description: This is a default description.
        type: post
  TransformSummary:
    properties:
      displayData:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      inputCollectionName:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      outputCollectionName:
        description: This is a default description.
        type: post
  WorkItem:
    properties:
      configuration:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      initialReportIndex:
        description: This is a default description.
        type: post
      jobId:
        description: This is a default description.
        type: post
      leaseExpireTime:
        description: This is a default description.
        type: post
      packages:
        description: This is a default description.
        type: post
      projectId:
        description: This is a default description.
        type: post
      reportStatusInterval:
        description: This is a default description.
        type: post
  WorkItemServiceState:
    properties:
      harnessData:
        description: This is a default description.
        type: post
      leaseExpireTime:
        description: This is a default description.
        type: post
      metricShortId:
        description: This is a default description.
        type: post
      nextReportIndex:
        description: This is a default description.
        type: post
      reportStatusInterval:
        description: This is a default description.
        type: post
  WorkItemStatus:
    properties:
      completed:
        description: This is a default description.
        type: post
      counterUpdates:
        description: This is a default description.
        type: post
      errors:
        description: This is a default description.
        type: post
      metricUpdates:
        description: This is a default description.
        type: post
      reportIndex:
        description: This is a default description.
        type: post
      requestedLeaseDuration:
        description: This is a default description.
        type: post
      workItemId:
        description: This is a default description.
        type: post
  WorkerHealthReport:
    properties:
      pods:
        description: This is a default description.
        type: post
      reportInterval:
        description: This is a default description.
        type: post
      vmIsHealthy:
        description: This is a default description.
        type: post
      vmStartupTime:
        description: This is a default description.
        type: post
  WorkerHealthReportResponse:
    properties:
      reportInterval:
        description: This is a default description.
        type: post
  WorkerMessage:
    properties:
      labels:
        description: This is a default description.
        type: post
      time:
        description: This is a default description.
        type: post
  WorkerMessageCode:
    properties:
      code:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
  WorkerMessageResponse:
    properties: []
  WorkerPool:
    properties:
      dataDisks:
        description: This is a default description.
        type: post
      defaultPackageSet:
        description: This is a default description.
        type: post
      diskSizeGb:
        description: This is a default description.
        type: post
      diskSourceImage:
        description: This is a default description.
        type: post
      diskType:
        description: This is a default description.
        type: post
      ipConfiguration:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      machineType:
        description: This is a default description.
        type: post
      metadata:
        description: This is a default description.
        type: post
      network:
        description: This is a default description.
        type: post
  WorkerSettings:
    properties:
      baseUrl:
        description: This is a default description.
        type: post
      reportingEnabled:
        description: This is a default description.
        type: post
      servicePath:
        description: This is a default description.
        type: post
      shuffleServicePath:
        description: This is a default description.
        type: post
      tempStoragePrefix:
        description: This is a default description.
        type: post
      workerId:
        description: This is a default description.
        type: post
  WriteInstruction:
    properties: []
x-collection-name: Google Dataflow
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