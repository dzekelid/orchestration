---
name: AWS CodeCommit
description: AWS CodeCommit is a fully-managed source control service that makes it
  easy for companies to host secure and highly scalable private Git repositories.
  CodeCommit eliminates the need to operate your own source control system or worry
  about scaling its infrastructure. You can use CodeCommit to securely store anything
  from source code to binaries, and it works seamlessly with your existing Git tools.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodeCommit.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Stack Network
- SDK
- Orchestration
- Amazon Web Services
created: "2018-02-25"
modified: "2018-02-25"
url: https://raw.githubusercontent.com/streamdata-gallery/orchestration/master/_listings/aws-codecommit/apis.yaml
specificationVersion: "0.14"
apis:
- name: AWS CodeCommit API
  description: AWS CodeCommit is a fully-managed source control service that makes
    it easy for companies to host secure and highly scalable private Git repositories
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodeCommit.png
  humanURL: ""
  baseURL: :///
  tags: Orchestration
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/orchestration/master/_listings/aws-codecommit/action-updaterepositoryname-get.md
x-common:
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/codecommit/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/codecommit/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/codecommit/faqs/
- type: x-getting-started
  url: ttps://aws.amazon.com/codecommit/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/codecommit/pricing/
- type: x-website
  url: https://aws.amazon.com/codecommit/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---