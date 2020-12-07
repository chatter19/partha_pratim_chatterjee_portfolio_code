---
date: 2019-08-19T10:58:08-04:00
description: "A tool that estimates data science salaries."
featured_image: "/images/iac-1.png"
title: "IaC Platform"
---

In my experience, one of the key factors that influence a company's velocity at whhich it can go to the market, is its ability to devise a platform that manages the infrastructure deployment of its clients.

In my current company, I had a similar task at hand, where i was to build a a cloud agnostic Infrastructure as Code platform (IaC Platform).

<!-- Some of the key things to consider on the tech front
---
* Tool(s) to automate infrasture deployment and configuration management
* Test strategy to prevent incorrect deployment of configuration
* A CI/CD pipeline to consume deployment triggers
* Tool to check apparant security vulnerabilities
* Tool to deply infrastrucutre and configuration for clients incrementally -->

Architecture Decisions
---
* Build a framework to import logically grouped modules (IaC module framework)
* Build a gateway to onboard clients seamlessly (IaC client framework)
* Version control infrasture and configuration states to facilitate incremantal updates

Tech Stack
---
* Terraform to automate infrastrucutre deployment.
* Ansible for configuration management.
* Kitchen Terraform to automate the testing strategy.
* Azure DevOps/Bitbucket Pipelines for building CI/CD pipeleine.
* Checkov to cover security and compliance best practices.
* Atlantis to automate pull requests on terraform files and apply configuration

<!-- {{< figure src="/images/iac-1.png" >}}
{{< figure src="/images/iac-2.png" >}}
{{< figure src="/images/iac-3.png" >}} -->

[Link to IaC module framework repository](https://github.com/chatter19/iac_modules)

[Link to IaC client framework repository](https://github.com/chatter19/iac_clients)
