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
  /?Action=SetLoadBasedAutoScaling&k=1:
    get:
      summary: ' Set Load Based Auto Scaling '
      description: Specify the load-based auto scaling configuration for a specified
        layer
      operationId: setLoadBasedAutoScaling
      parameters:
      - in: query
        name: DownScaling
        description: An AutoScalingThresholds object with the downscaling threshold
          configuration
        type: string
      - in: query
        name: Enable
        description: Enables load-based auto scaling for the layer
        type: string
      - in: query
        name: LayerId
        description: The layer ID
        type: string
      - in: query
        name: UpScaling
        description: An AutoScalingThresholds object with the upscaling threshold
          configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - auto scaling
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