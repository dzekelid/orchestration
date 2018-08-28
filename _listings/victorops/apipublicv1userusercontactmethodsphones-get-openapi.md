---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 0
info:
  title: VictorOps Get a list of all contact phones for a user
  description: |-
    Get the contact phones for a user

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
  /api-public/v1/profile/{username}/policies/{step}:
    get:
      summary: Get a paging policy step
      description: |-
        Get a paging policy step

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.profile.username.policies.step.get
      x-api-path-slug: apipublicv1profileusernamepoliciesstep-get
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
      - Step
    post:
      summary: Create a rule for a paging policy step
      description: |-
        Create a rule for a paging policy step

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.profile.username.policies.step.post
      x-api-path-slug: apipublicv1profileusernamepoliciesstep-post
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
      - Step
    put:
      summary: Update a paging policy step
      description: |-
        Update a paging policy step

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.profile.username.policies.step.put
      x-api-path-slug: apipublicv1profileusernamepoliciesstep-put
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
      - Step
  /api-public/v1/profile/{username}/policies/{step}/{rule}:
    delete:
      summary: Delete a rule from a paging policy step
      description: |-
        Delete a rule from a paging policy step

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.profile.username.policies.step.rule.delete
      x-api-path-slug: apipublicv1profileusernamepoliciessteprule-delete
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
      - Step
      - Rule
    get:
      summary: Get a rule from a paging policy step
      description: |-
        Get a rule from a paging policy step

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.profile.username.policies.step.rule.get
      x-api-path-slug: apipublicv1profileusernamepoliciessteprule-get
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
      - Step
      - Rule
    put:
      summary: Update a rule for a paging policy step
      description: |-
        Update a rule for a paging policy step

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.profile.username.policies.step.rule.put
      x-api-path-slug: apipublicv1profileusernamepoliciessteprule-put
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
      - Step
      - Rule
  /api-public/v1/team:
    get:
      summary: List teams
      description: |-
        Get a list of teams for your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.get
      x-api-path-slug: apipublicv1team-get
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
      - Team
    post:
      summary: Add a team
      description: |-
        Add a team to your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.post
      x-api-path-slug: apipublicv1team-post
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
      - Team
  /api-public/v1/team/{team}:
    delete:
      summary: Remove a team
      description: |-
        Remove a team from your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.delete
      x-api-path-slug: apipublicv1teamteam-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to be deleted
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Team
      - Team
    get:
      summary: Retrieve information for a team
      description: |-
        Get the information for the specified team.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.get
      x-api-path-slug: apipublicv1teamteam-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to fetch
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Team
      - Team
    put:
      summary: Update a team
      description: |-
        Update the designated team

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.put
      x-api-path-slug: apipublicv1teamteam-put
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to be updated
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Team
      - Team
  /api-public/v1/team/{team}/members:
    get:
      summary: Retrieve a list of members for a team
      description: |-
        Get the members for the specified team.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.members.get
      x-api-path-slug: apipublicv1teamteammembers-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to fetch
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Team
      - Team
      - Members
    post:
      summary: Add a team member
      description: |-
        Add a team member to your team.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.members.post
      x-api-path-slug: apipublicv1teamteammembers-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to fetch
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Team
      - Team
      - Members
  /api-public/v1/team/{team}/members/{user}:
    delete:
      summary: Remove a team member
      description: |-
        Remove a team from your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.members.user.delete
      x-api-path-slug: apipublicv1teamteammembersuser-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to be deleted
      - in: path
        name: user
        description: The team member username
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Team
      - Team
      - Members
      - User
  /api-public/v1/team/{team}/oncall/schedule:
    get:
      summary: Get a team's on-call schedule
      description: |-
        __NOTE: This call is deprecated. Please use `GET /api-public/v2/team/{team}/oncall/schedule`.__

        Get the on-call schedule for a team, including on-call overrides.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.oncall.schedule.get
      x-api-path-slug: apipublicv1teamteamoncallschedule-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team slug
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Team
      - Team
      - Oncall
      - Schedule
  /api-public/v1/team/{team}/oncall/user:
    patch:
      summary: Create an on-call override (take on-call)
      description: |-
        __NOTE: This API call is deprecated. Please use `PATCH /api-public/v2/policies/{policy}/oncall/user`__

        Replaces a currently on-call user on the team with another.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.team.team.oncall.user.patch
      x-api-path-slug: apipublicv1teamteamoncalluser-patch
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team slug
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Team
      - Team
      - Oncall
      - User
  /api-public/v1/team/{team}/policies:
    get:
      summary: Retrieve a list of escalation policies for a team
      description: |-
        Get the escalation policies for the specified team.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.policies.get
      x-api-path-slug: apipublicv1teamteampolicies-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to fetch
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Team
      - Team
      - Policies
  /api-public/v1/user:
    get:
      summary: List users
      description: |-
        Get a list of users for your organization

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.get
      x-api-path-slug: apipublicv1user-get
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
      - User
    post:
      summary: Add a user
      description: |-
        Add a user to your organization

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.post
      x-api-path-slug: apipublicv1user-post
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
      - User
  /api-public/v1/user/{user}:
    delete:
      summary: Remove a user
      description: |-
        Remove a user from your organization

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.delete
      x-api-path-slug: apipublicv1useruser-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user to be deleted
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
    get:
      summary: Retrieve information for a user
      description: |-
        Get the information for the specified user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.get
      x-api-path-slug: apipublicv1useruser-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user to fetch
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
    put:
      summary: Update a user
      description: |-
        Update the designated user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.put
      x-api-path-slug: apipublicv1useruser-put
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user to be updated
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
  /api-public/v1/user/{user}/contact-methods:
    get:
      summary: Get a list of all contact methods for a user
      description: |-
        Get the contact methods for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.get
      x-api-path-slug: apipublicv1userusercontactmethods-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
      - Contact-methods
  /api-public/v1/user/{user}/contact-methods/devices:
    get:
      summary: Get a list of all contact devices for a user
      description: |-
        Get the contact methods for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.devices.get
      x-api-path-slug: apipublicv1userusercontactmethodsdevices-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
      - Contact-methods
      - Devices
  /api-public/v1/user/{user}/contact-methods/devices/{contactId}:
    delete:
      summary: Delete a contact device for a user
      description: |-
        Delete a contact device for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.devices.contactId.delete
      x-api-path-slug: apipublicv1userusercontactmethodsdevicescontactid-delete
      parameters:
      - in: path
        name: contactId
        description: The unique contact identifier
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
      - Contact-methods
      - Devices
      - ContactId
    get:
      summary: Get the indicated contact device for a user
      description: |-
        Get the indicated contact device for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.devices.contactId.get
      x-api-path-slug: apipublicv1userusercontactmethodsdevicescontactid-get
      parameters:
      - in: path
        name: contactId
        description: The unique contact identifier
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
      - Contact-methods
      - Devices
      - ContactId
    put:
      summary: Update a contact device for a user
      description: |-
        Update a contact device for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.devices.contactId.put
      x-api-path-slug: apipublicv1userusercontactmethodsdevicescontactid-put
      parameters:
      - in: path
        name: contactId
        description: The unique contact identifier
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
      - Contact-methods
      - Devices
      - ContactId
  /api-public/v1/user/{user}/contact-methods/emails:
    get:
      summary: Get a list of all contact emails for a user
      description: |-
        Get the contact emails for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.emails.get
      x-api-path-slug: apipublicv1userusercontactmethodsemails-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
      - Contact-methods
      - Emails
    post:
      summary: Create a contact emails for a user
      description: |-
        Create a contact email for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.emails.post
      x-api-path-slug: apipublicv1userusercontactmethodsemails-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
      - Contact-methods
      - Emails
  /api-public/v1/user/{user}/contact-methods/emails/{contactId}:
    delete:
      summary: Delete a contact email for a user
      description: |-
        Delete the indicated contact email for the user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.emails.contactId.delete
      x-api-path-slug: apipublicv1userusercontactmethodsemailscontactid-delete
      parameters:
      - in: path
        name: contactId
        description: The unique contact identifier
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
      - Contact-methods
      - Emails
      - ContactId
    get:
      summary: Get the indicate contact email for a user
      description: |-
        Get the indicated contact email for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.emails.contactId.get
      x-api-path-slug: apipublicv1userusercontactmethodsemailscontactid-get
      parameters:
      - in: path
        name: contactId
        description: The unique contact identifier
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
      - Contact-methods
      - Emails
      - ContactId
  /api-public/v1/user/{user}/contact-methods/phones:
    get:
      summary: Get a list of all contact phones for a user
      description: |-
        Get the contact phones for a user

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.contact_methods.phones.get
      x-api-path-slug: apipublicv1userusercontactmethodsphones-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - User
      - User
      - Contact-methods
      - Phones
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