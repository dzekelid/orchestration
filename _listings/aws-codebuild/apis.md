---
name: AWS CodeBuild
description: AWS CodeBuild is a fully managed build service that compiles source code,
  runs tests, and produces software packages that are ready to deploy. With CodeBuild,
  you donrsquo;t need to provision, manage, and scale your own build servers. CodeBuild
  scales continuously and processes multiple builds concurrently, so your builds are
  not left waiting in a queue. You can get started quickly by using prepackaged build
  environments, or you can create custom build environments that use your own build
  tools. With CodeBuild, you are charged by the minute for the compute resources you
  use.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-build-console-icon.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Stack Network
- SDK
- Orchestration
- Amazon Web Services
created: "2018-02-25"
modified: "2018-02-25"
url: https://raw.githubusercontent.com/streamdata-gallery/orchestration/master/_listings/aws-codebuild/apis.yaml
specificationVersion: "0.14"
apis:
- name: AWS CodeBuild API
  description: AWS CodeBuild is a fully managed build service that compiles source
    code, runs tests, and produces software packages that are ready to deploy
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-build-console-icon.png
  humanURL: ""
  baseURL: :///
  tags: Orchestration
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/orchestration/master/_listings/aws-codebuild/action-updateproject-get.md
x-common:
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/codebuild/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/codebuild/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/codebuild/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/codebuild/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/codebuild/pricing/
- type: x-website
  url: https://aws.amazon.com/codebuild/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---