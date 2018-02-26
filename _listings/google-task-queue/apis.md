---
name: Google Task Queue
description: The Task Queue API lets applications perform work, called tasks, asynchronously
  outside of a user request. If an app needs to execute work in the background, it
  adds tasks to task queues. The tasks are executed later, by scalable App Engine
  worker services in your application.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hands-on-app-engine-11-638.jpg
x-kinRank: "9"
x-alexaRank: ""
tags:
- Tasks
- Stack Network
- Orchestration
- Jobs
- Google APIs
created: "2018-02-25"
modified: "2018-02-25"
url: https://raw.githubusercontent.com/streamdata-gallery/orchestration/master/_listings/google-task-queue/apis.yaml
specificationVersion: "0.14"
apis:
- name: Google Task Queue API
  description: The Task Queue API lets applications perform work, called tasks, asynchronously
    outside of a user request
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hands-on-app-engine-11-638.jpg
  humanURL: ""
  baseURL: ://www.googleapis.com//taskqueue/v1beta2/projects
  tags: Orchestration
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/orchestration/master/_listings/google-task-queue/project-taskqueues-taskqueue-tasks-task-post.md
x-common:
- type: x-code
  url: https://cloud.google.com/appengine/docs/standard/python/taskqueue/rest/libraries
- type: x-documentation
  url: https://cloud.google.com/appengine/docs/standard/python/taskqueue/rest/
- type: x-performance
  url: https://cloud.google.com/appengine/docs/standard/python/taskqueue/rest/performance
- type: x-website
  url: https://cloud.google.com/appengine/docs/standard/python/taskqueue/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---