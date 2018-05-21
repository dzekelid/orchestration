---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 0
info:
  title: VictorOps Get current incident information
  description: |-
    Get a list of the currently open, acknowledged and recently resolved incidents.
    This API may be called a maximum of 6 times per minute.
  version: 1.0.0
host: api.victorops.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-public/v1/alerts/{uuid}:
    get:
      summary: Retrieve alert details.
      description: |-
        Retrieve the details of an alert that was sent VictorOps by you.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.alerts.uuid.get
      x-api-path-slug: apipublicv1alertsuuid-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: uuid
        description: The VictorOps uuid of the alert
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Alerts
      - Uuid
  /api-public/v1/incidents:
    get:
      summary: Get current incident information
      description: |-
        Get a list of the currently open, acknowledged and recently resolved incidents.
        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.get
      x-api-path-slug: apipublicv1incidents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Incidents
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