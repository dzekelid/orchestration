---
swagger: "2.0"
info:
  title: Cloud Source Repositories
  description: Access source code repositories hosted by Google.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: sourcerepo.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set Access Control Policy
      description: Sets the access control policy on the specified resource
      operationId: sourcerepo.projects.repos.setIamPolicy
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being specified'
      responses:
        200:
          description: OK
      tags:
      - repository policy
definitions:
  AuditConfig:
    properties:
      auditLogConfigs:
        description: This is a default description.
        type: post
      exemptedMembers:
        description: This is a default description.
        type: post
      service:
        description: This is a default description.
        type: post
  AuditLogConfig:
    properties:
      exemptedMembers:
        description: This is a default description.
        type: post
      logType:
        description: This is a default description.
        type: post
  Binding:
    properties:
      members:
        description: This is a default description.
        type: post
      role:
        description: This is a default description.
        type: post
  CloudAuditOptions:
    properties: []
  Condition:
    properties:
      iam:
        description: This is a default description.
        type: post
      op:
        description: This is a default description.
        type: post
      svc:
        description: This is a default description.
        type: post
      sys:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
      values:
        description: This is a default description.
        type: post
  CounterOptions:
    properties:
      field:
        description: This is a default description.
        type: post
      metric:
        description: This is a default description.
        type: post
  DataAccessOptions:
    properties: []
  Empty:
    properties: []
  ListReposResponse:
    properties:
      repos:
        description: This is a default description.
        type: post
  LogConfig:
    properties: []
  MirrorConfig:
    properties:
      deployKeyId:
        description: This is a default description.
        type: post
      url:
        description: This is a default description.
        type: post
      webhookId:
        description: This is a default description.
        type: post
  Policy:
    properties:
      auditConfigs:
        description: This is a default description.
        type: post
      bindings:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
      iamOwned:
        description: This is a default description.
        type: post
      rules:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
  Repo:
    properties:
      name:
        description: This is a default description.
        type: post
      size:
        description: This is a default description.
        type: post
      url:
        description: This is a default description.
        type: post
  Rule:
    properties:
      action:
        description: This is a default description.
        type: post
      conditions:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      in:
        description: This is a default description.
        type: post
      logConfig:
        description: This is a default description.
        type: post
      notIn:
        description: This is a default description.
        type: post
      permissions:
        description: This is a default description.
        type: post
  SetIamPolicyRequest:
    properties:
      updateMask:
        description: This is a default description.
        type: post
  TestIamPermissionsRequest:
    properties:
      permissions:
        description: This is a default description.
        type: post
  TestIamPermissionsResponse:
    properties:
      permissions:
        description: This is a default description.
        type: post
x-collection-name: Google Cloud Source Repositories
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