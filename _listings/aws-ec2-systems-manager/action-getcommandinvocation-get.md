---
swagger: "2.0"
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetCommandInvocation&k=1:
    get:
      summary: ' Get Command Invocation '
      description: Returns detailed information about command execution for an invocation
        or plugin
      operationId: getCommandInvocation
      parameters:
      - in: query
        name: CommandId
        description: (Required) The parent command ID of the invocation plugin
        type: string
      - in: query
        name: InstanceId
        description: (Required) The ID of the managed instance targeted by the command
        type: string
      - in: query
        name: PluginName
        description: (Optional) The name of the plugin for which you want detailed
          results
        type: string
      responses:
        200:
          description: OK
      tags:
      - command invocation
definitions: []
x-collection-name: AWS EC2 Systems Manager
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