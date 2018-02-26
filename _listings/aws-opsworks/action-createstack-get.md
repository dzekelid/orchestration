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
  /?Action=CreateStack&k=1:
    get:
      summary: ' Create Stack '
      description: Creates a new stack
      operationId: createStack
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
        description: The stack's default Availability Zone, which must be in the specified
          region
        type: string
      - in: query
        name: DefaultInstanceProfileArn
        description: The Amazon Resource Name (ARN) of an IAM profile that is the
          default profile for all of the stack's EC2 instances
        type: string
      - in: query
        name: DefaultOs
        description: The stack's default operating system, which is installed on every
          instance unless you specify a different operating system when you create
          the instance
        type: string
      - in: query
        name: DefaultRootDeviceType
        description: The default root device type
        type: string
      - in: query
        name: DefaultSshKeyName
        description: A default Amazon EC2 key pair name
        type: string
      - in: query
        name: DefaultSubnetId
        description: The stack's default VPC subnet ID
        type: string
      - in: query
        name: HostnameTheme
        description: The stack's host name theme, with spaces replaced by underscores
        type: string
      - in: query
        name: Name
        description: The stack name
        type: string
      - in: query
        name: Region
        description: The stack's AWS region, such as ap-south-1
        type: string
      - in: query
        name: ServiceRoleArn
        description: The stack's AWS Identity and Access Management (IAM) role, which
          allows AWS OpsWorks Stacks to work with AWS      resources on your behalf
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
      - in: query
        name: VpcId
        description: The ID of the VPC that the stack is to be launched into
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
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