---
title: devops is adding value to software products
date: 2022-10-18
author: socdev
---

how devops adds value to software products:

- by automation (Ansible, Terraform, etc.)
- by streamlining workflows/identifying bottlenecks
- ...

## typical risks in software lifecycle

|risk|mitigation|
|-|-|
|outdated documentation|automate documentation generation|
|unclear responsabilities between teams/actors|?|
|manual interventions and handoffs|automation and self-service tools|
|unauthorized/unintentional configuration changes|infrastructure and configurations as code|
|inconsistensies between dev/qa/production environments|_idem_|
|unable to diagnose issues with incomplete, scattered, logs and traces|implement built-in observability|
|manual incident management can cause delays|automate incident notifications into communication channels|

### development stage

#### onboarding and tools

- every actor requires Slack Exchange access
- source control: automate GitLab account management
- cloud environment: AWS developer account
- provisioning: provisioning development environments and tools (
  documentation and guidelines)
- local environment: IDE, text editor, and dependencies (docker, linters, web
  server, etc.)

## integration and testing stages

- code review process
  - GitLab web app
  - static code analysis (sonarqube, esLint, etc.)
- dependency management
  - maven, nuget, npm, pip, etc. 
- security scans
- build management
  - Gitlab CI + runners, etc. (Jenkins, gradle, bamboo, travis) 
- artifact management repository
- QA environment (deploying artifact to QA envir)
- functional testing
- workflow management
  - GitLab (Jira, Trello, Asana, etc.) 

## deployment (release) stage

- performance testing (against regression)
  - webload, jMeter, loadninja, loadrunner, etc.
- containerization
  - docker, rkt, mesos
  - docker compose vs. Ansible
- cloud deployment 
  - avoid vendor lock-in(really?)

## monitoring and analytics stage

- gathering logs
  - splunk, elasticsearch => searching, reporting purposes
  - log aggregation
- using logs and data to build dashboards
- observability
  - datadog, new relic, honeycomb, dynatrace
- monitoring
- incident management and collaboration 