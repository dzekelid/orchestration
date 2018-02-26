---
name: AWS Step Functions
description: AWS Step Functions makes it easy to coordinate the components of distributed
  applications and microservices using visual workflows. Building applications from
  individual components that each perform a discrete function lets you scale and change
  applications quickly. Step Functions is a reliable way to coordinate components
  and step through the functions of your application. Step Functions provides a graphical
  console to arrange and visualize the components of your application as a series
  of steps. This makes it simple to build and run multi-step applications. Step Functions
  automatically triggers and tracks each step, and retries when there are errors,
  so your application executes in order and as expected. Step Functions logs the state
  of each step, so when things do go wrong, you can diagnose and debug problems quickly.
  You can change and add steps without even writing code, so you can easily evolve
  your application and innovate faster.nnAWS Step Functions manages the operations
  and underlying infrastructure for you to help ensure your application is available
  at any scale.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-step-functions.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Stack Network
- Orchestration
- iPaaS
- Etl
- Automation
- Amazon Web Services
created: "2018-02-25"
modified: "2018-02-25"
url: https://raw.githubusercontent.com/streamdata-gallery/orchestration/master/_listings/aws-step-functions/apis.yaml
specificationVersion: "0.14"
apis:
- name: AWS Step Functions API
  description: AWS Step Functions makes it easy to coordinate the components of distributed
    applications and microservices using visual workflows
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-step-functions.png
  humanURL: ""
  baseURL: :///
  tags: Orchestration
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/orchestration/master/_listings/aws-step-functions/action-stopexecution-get.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/step-functions/latest/apireference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/step-functions/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/step-functions/getting-started/
- type: x-how-it-works
  url: https://aws.amazon.com/step-functions/#howitworks
- type: x-pricing
  url: https://aws.amazon.com/step-functions/pricing/
- type: x-website
  url: https://aws.amazon.com/step-functions/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---