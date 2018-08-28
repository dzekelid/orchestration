---
swagger: "2.0"
info:
  title: AWS CodeBuild API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartBuild&k=1:
    get:
      summary: ' Start Build '
      description: Starts running a build
      operationId: startBuild
      parameters:
      - in: query
        name: artifactsOverride
        description: Build output artifact settings that override, for this build
          only, the latest ones already defined in the corresponding build project
        type: string
      - in: query
        name: buildspecOverride
        description: A build spec declaration that overrides, for this build only,
          the latest one already defined in the corresponding build project
        type: string
      - in: query
        name: environmentVariablesOverride
        description: A set of environment variables that overrides, for this build
          only, the latest ones already defined in the corresponding build project
        type: string
      - in: query
        name: projectName
        description: The name of the build project to start running a build
        type: string
      - in: query
        name: sourceVersion
        description: A version of the build input to be built, for this build only
        type: string
      - in: query
        name: timeoutInMinutesOverride
        description: The number of build timeout minutes, from 5 to 480 (8 hours)
          that overrides, for this build only, the latest setting already defined
          in the corresponding build project
        type: string
      responses:
        200:
          description: OK
      tags:
      - builds
definitions: []
x-collection-name: AWS CodeBuild
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