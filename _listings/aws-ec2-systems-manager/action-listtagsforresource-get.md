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
  /?Action=ListTagsForResource&k=1:
    get:
      summary: ' List Tags For Resource '
      description: Returns a list of the tags assigned to the specified resource
      operationId: listTagsForResource
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID for which you want to see a list of tags
        type: string
      - in: query
        name: ResourceType
        description: Returns a list of tags for a specific resource type
        type: string
      responses:
        200:
          description: OK
      tags:
      - resource tags
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