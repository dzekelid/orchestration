---
swagger: "2.0"
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateInstance&k=1:
    get:
      summary: ' Update Instance '
      description: Updates a specified instance
      operationId: updateInstance
      parameters:
      - in: query
        name: AgentVersion
        description: The default AWS OpsWorks Stacks agent version
        type: string
      - in: query
        name: AmiId
        description: The ID of the AMI that was used to create the instance
        type: string
      - in: query
        name: Architecture
        description: The instance architecture
        type: string
      - in: query
        name: AutoScalingType
        description: For load-based or time-based instances, the type
        type: string
      - in: query
        name: EbsOptimized
        description: This property cannot be updated
        type: string
      - in: query
        name: Hostname
        description: The instance host name
        type: string
      - in: query
        name: InstallUpdatesOnBoot
        description: Whether to install operating system and package updates when
          the instance boots
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: InstanceType
        description: The instance type, such as t2
        type: string
      - in: query
        name: LayerIds
        description: The instance's layer IDs
        type: string
      - in: query
        name: Os
        description: The instance's operating system, which must be set to one of
          the following
        type: string
      - in: query
        name: SshKeyName
        description: The instance's Amazon EC2 key name
        type: string
      responses:
        200:
          description: OK
      tags:
      - instances
definitions: []
x-collection-name: AWS OpsWorks
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