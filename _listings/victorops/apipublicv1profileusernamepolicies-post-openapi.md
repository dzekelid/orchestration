---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 0
info:
  title: VictorOps Create a paging policy step
  description: |-
    Create a paging policy step

    This API may be called a maximum of 15 times per minute.
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
    post:
      summary: Create a new incident
      description: |-
        Create a new incident.

        This call replicates the function of our
        manual incident creation process.
        Monitoring tools and custom integrations
        should be configured using our
        REST Endpoint.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.post
      x-api-path-slug: apipublicv1incidents-post
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
  /api-public/v1/incidents/ack:
    patch:
      summary: Acknowledge an incident or list of incidents
      description: |-
        The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.ack.patch
      x-api-path-slug: apipublicv1incidentsack-patch
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
      - Ack
  /api-public/v1/incidents/byUser/ack:
    patch:
      summary: Acknowledge all incidents for which a user was paged.
      description: |-
        The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.byUser.ack.patch
      x-api-path-slug: apipublicv1incidentsbyuserack-patch
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
      - ByUser
      - Ack
  /api-public/v1/incidents/byUser/resolve:
    patch:
      summary: Resolve all incidents for which a user was paged.
      description: |-
        The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.byUser.resolve.patch
      x-api-path-slug: apipublicv1incidentsbyuserresolve-patch
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
      - ByUser
      - Resolve
  /api-public/v1/incidents/reroute:
    post:
      summary: Reroute one or more incidents to one or more new routable destinations.
      description: Reroute one or more incidents to one or more users and/or escalation
        policies
      operationId: api_public.v1.incidents.reroute.post
      x-api-path-slug: apipublicv1incidentsreroute-post
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
      - Reroute
  /api-public/v1/incidents/resolve:
    patch:
      summary: Resolve an incident or list of incidents
      description: |-
        The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.resolve.patch
      x-api-path-slug: apipublicv1incidentsresolve-patch
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
      - Resolve
  /api-public/v1/oncall/current:
    get:
      summary: Get an organization's on-call users
      description: |-
        Get all on-call uesrs/teams for your organization.

        This API may be called a maximum of 1 times per minute.
      operationId: api_public.v1.oncall.current.get
      x-api-path-slug: apipublicv1oncallcurrent-get
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
      - Oncall
      - Current
  /api-public/v1/org/routing-keys:
    get:
      summary: List routing keys with associated teams
      description: |-
        Retrieves a list of routing keys and associated teams.
        This API may be called a maximum of once a minute.
      operationId: api_public.v1.org.routing_keys.get
      x-api-path-slug: apipublicv1orgroutingkeys-get
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
      - Org
      - Routing-keys
  /api-public/v1/policies:
    get:
      summary: Get escalation policy info
      description: |-
        Retrieves a list of escalation policy information.
        This API may be called a maximum of once a minute
      operationId: api_public.v1.policies.get
      x-api-path-slug: apipublicv1policies-get
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
      - Policies
  /api-public/v1/policies/types/contacts:
    get:
      summary: Get the available contact types
      description: |-
        Get the available contact types

        description: "Email Address", type: "email"
        description: "Phone Number", type: "phone"

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.policies.types.contacts.get
      x-api-path-slug: apipublicv1policiestypescontacts-get
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
      - Policies
      - Types
      - Contacts
  /api-public/v1/policies/types/notifications:
    get:
      summary: Get the available notification types
      description: |-
        Get the available notification types

        description: "Send a push notification to all my devices", type: "push"
        description: "Send an email to an email address", type: "email"
        description: "Send an SMS to a phone number", type: "sms"
        description: "Make a phone call to a phone number", type: "phone"

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.policies.types.notifications.get
      x-api-path-slug: apipublicv1policiestypesnotifications-get
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
      - Policies
      - Types
      - Notifications
  /api-public/v1/policies/types/timeouts:
    get:
      summary: Get the available timeout values
      description: |-
        Get the available timeout values

        description: "If still unacked after 1 minute", type: 1
        description: "If still unacked after 5 minutes", type: 5
        description: "If still unacked after 10 minutes", type: 10
        description: "If still unacked after 15 minutes", type: 15
        description: "If still unacked after 20 minutes", type: 20
        description: "If still unacked after 25 minutes", type: 25
        description: "If still unacked after 30 minutes", type: 30
        description: "If still unacked after 45 minutes", type: 45
        description: "If still unacked after 60 minutes", type: 60

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.policies.types.timeouts.get
      x-api-path-slug: apipublicv1policiestypestimeouts-get
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
      - Policies
      - Types
      - Timeouts
  /api-public/v1/policies/{policy}/oncall/user:
    patch:
      summary: Create an on-call override (take on-call)
      description: |-
        Replaces a currently on-call user in the escalation policy with another.  In many cases, the policy slug
        will match the slug of the team that contains it.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.policies.policy.oncall.user.patch
      x-api-path-slug: apipublicv1policiespolicyoncalluser-patch
      parameters:
      - in: query
        name: No Name
      - in: path
        name: policy
        description: The VictorOps policy slug
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Policies
      - Policy
      - Oncall
      - User
  /api-public/v1/profile/{username}/policies:
    get:
      summary: Get the user's paging policy
      description: |-
        Get all the paging policy steps for the user on the org associated with the API key

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.profile.username.policies.get
      x-api-path-slug: apipublicv1profileusernamepolicies-get
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
      - Profile
      - Username
      - Policies
    post:
      summary: Create a paging policy step
      description: |-
        Create a paging policy step

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.profile.username.policies.post
      x-api-path-slug: apipublicv1profileusernamepolicies-post
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
      - Profile
      - Username
      - Policies
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