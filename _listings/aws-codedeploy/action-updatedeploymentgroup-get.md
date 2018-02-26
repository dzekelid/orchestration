---
swagger: "2.0"
info:
  title: AWS CodeDeploy API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateDeploymentGroup&k=1:
    get:
      summary: ' Update Deployment Group '
      description: Changes information about a deployment group
      operationId: updateDeploymentGroup
      parameters:
      - in: query
        name: alarmConfiguration
        description: Information to add or change about Amazon CloudWatch alarms when
          the deployment            group is updated
        type: string
      - in: query
        name: applicationName
        description: The application name corresponding to the deployment group to
          update
        type: string
      - in: query
        name: autoRollbackConfiguration
        description: Information for an automatic rollback configuration that is added
          or changed when a            deployment group is updated
        type: string
      - in: query
        name: autoScalingGroups
        description: The replacement list of Auto Scaling groups to be included in
          the deployment group,            if you want to change them
        type: string
      - in: query
        name: currentDeploymentGroupName
        description: The current name of the deployment group
        type: string
      - in: query
        name: deploymentConfigName
        description: The replacement deployment configuration name to use, if you
          want to change            it
        type: string
      - in: query
        name: ec2TagFilters
        description: The replacement set of Amazon EC2 tags on which to filter, if
          you want to change            them
        type: string
      - in: query
        name: newDeploymentGroupName
        description: The new name of the deployment group, if you want to change it
        type: string
      - in: query
        name: onPremisesInstanceTagFilters
        description: The replacement set of on-premises instance tags on which to
          filter, if you want to            change them
        type: string
      - in: query
        name: serviceRoleArn
        description: A replacement ARN for the service role, if you want to change
          it
        type: string
      - in: query
        name: triggerConfigurations
        description: Information about triggers to change when the deployment group
          is updated
        type: string
      responses:
        200:
          description: OK
      tags:
      - deployment groups
definitions: []
x-collection-name: AWS CodeDeploy
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