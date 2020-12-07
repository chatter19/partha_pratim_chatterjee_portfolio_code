---
date: 2020-02-19T12:58:08-04:00
description: "A tool that estimates data science salaries."
featured_image: "/images/ready_to_work.png"
title: "Ready To Work: A covid Initiative"
---

In the current COVID hit world, it is necessary to understand wether employees are fit to go back to work. 
I developed a pluggable interface, 
* that consumes a survey response in the form of json, 
* queues it to our AI to calculate the odds for or against a person going back to work and 
* sends out those results to a web screen

Architecture Decisions
---
* One monolithic application over microservices.
* Test strategy to impolement unit and integration tests.
* Performance Optimisation
* A CI/CD pipeline to consume deployment triggers.

Tech Decisions
---
* Microservices to logically group the REST services and enable isolated deployment of these endpoints.
* Azure functions to develop and deploy endpoints and message queuing in Blob containers
* Consume incoming requests, calculate odds and send out results asynschronusly to optimise performance. 
* Pytest framework to implement unit testing and integration testing.
* Azure DevOps/Bitbucket Pipelines for building CI/CD pipeleine.

Additional Features
---
* Containarized scoring
* Custom logging on Application insights


<!-- {{< figure src="/images/ready_to_work.png" >}} -->

<!-- [Link to GitHub Repository](https://github.com/PlayingNumbers/ds_salary_proj) -->
