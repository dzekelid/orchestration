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
  /?Action=UpdateStack&k=1:
    get:
      summary: ' Update Stack '
      description: Updates a specified stack
      operationId: updateStack
      parameters:
      - in: query
        name: AgentVersion
        description: The default AWS OpsWorks Stacks agent version
        type: string
      - in: query
        name: Attributes
        description: One or more user-defined key-value pairs to be added to the stack
          attributes
        type: string
      - in: query
        name: ChefConfiguration
        description: A ChefConfiguration object that specifies whether to enable Berkshelf
          and the      Berkshelf version on Chef 11
        type: string
      - in: query
        name: ConfigurationManager
        description: The configuration manager
        type: string
      - in: query
        name: CustomCookbooksSource
        description: Contains the information required to retrieve an app or cookbook
          from a repository
        type: string
      - in: query
        name: CustomJson
        description: A string that contains user-defined, custom JSON
        type: string
      - in: query
        name: DefaultAvailabilityZone
        description: The stack's default Availability Zone, which must be in the      stack's
          region
        type: string
      - in: query
        name: DefaultInstanceProfileArn
        description: The ARN of an IAM profile that is the default profile for all
          of the stack's EC2 instances
        type: string
      - in: query
        name: DefaultOs
        description: 'The stack''s operating system, which must be set to one of the
          following:'
        type: string
      - in: query
        name: DefaultRootDeviceType
        description: The default root device type
        type: string
      - in: query
        name: DefaultSshKeyName
        description: A default Amazon EC2 key-pair name
        type: string
      - in: query
        name: DefaultSubnetId
        description: The stack's default VPC subnet ID
        type: string
      - in: query
        name: HostnameTheme
        description: The stack's new host name theme, with spaces replaced by underscores
        type: string
      - in: query
        name: Name
        description: The stack's new name
        type: string
      - in: query
        name: ServiceRoleArn
        description: Do not use this parameter
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      - in: query
        name: UseCustomCookbooks
        description: Whether the stack uses custom cookbooks
        type: string
      - in: query
        name: UseOpsworksSecurityGroups
        description: Whether to associate the AWS OpsWorks Stacks built-in security
          groups with the stack's layers
        type: string
      responses:
        200:
          description: OK
      tags:
      - stacks
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