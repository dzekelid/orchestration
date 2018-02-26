---
name: AWS X-Ray
description: AWS X-Ray helps developers analyze and debug production, distributed
  applications, such as those built using a microservices architecture. With X-Ray,
  you can understand how your application and its underlying services are performing
  to identify and troubleshoot the root cause of performance issues and errors. X-Ray
  provides an end-to-end view of requests as they travel through your application,
  and shows a map of your applications underlying components. You can use X-Ray to
  analyze both applications in development and in production, from simple three-tier
  applications to complex microservices applications consisting of thousands of services.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-xray.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Testing
- Stack Network
- Orchestration
- Monitoring
- Amazon Web Services
created: "2018-02-25"
modified: "2018-02-25"
url: https://raw.githubusercontent.com/streamdata-gallery/orchestration/master/_listings/aws-xray/apis.yaml
specificationVersion: "0.14"
apis:
- name: AWS X-Ray API
  description: AWS X-Ray helps developers analyze and debug production, distributed
    applications, such as those built using a microservices architecture
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-xray.png
  humanURL: ""
  baseURL: :///
  tags: Orchestration
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/orchestration/master/_listings/aws-xray/action-puttracesegments-get.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/xray/latest/api/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/xray/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/xray/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/xray/pricing/
- type: x-website
  url: https://aws.amazon.com/xray/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---