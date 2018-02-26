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
  /?Action=UpdateApp&k=1:
    get:
      summary: ' Update App '
      description: Updates a specified app
      operationId: updateApp
      parameters:
      - in: query
        name: AppId
        description: The app ID
        type: string
      - in: query
        name: AppSource
        description: A Source object that specifies the app repository
        type: string
      - in: query
        name: Attributes
        description: One or more user-defined key/value pairs to be added to the stack
          attributes
        type: string
      - in: query
        name: DataSources
        description: The app's data sources
        type: string
      - in: query
        name: Description
        description: A description of the app
        type: string
      - in: query
        name: Domains
        description: The app's virtual host settings, with multiple domains separated
          by commas
        type: string
      - in: query
        name: EnableSsl
        description: Whether SSL is enabled for the app
        type: string
      - in: query
        name: Environment
        description: An array of EnvironmentVariable objects that specify environment
          variables to be      associated with the app
        type: string
      - in: query
        name: Name
        description: The app name
        type: string
      - in: query
        name: SslConfiguration
        description: An SslConfiguration object with the SSL configuration
        type: string
      - in: query
        name: Type
        description: The app type
        type: string
      responses:
        200:
          description: OK
      tags:
      - applications
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