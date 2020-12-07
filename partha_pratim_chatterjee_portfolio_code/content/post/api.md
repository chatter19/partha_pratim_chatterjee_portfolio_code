---
date: 2020-10-17T13:58:08-04:00
description: "A tool that estimates data science salaries."
featured_image: "/images/api-1.png"
title: "One API to rule them all"
---

To further assist 'going to market' strategies, it is imperative from a technical standpoint to have an application interface to perform the proverbial 'CRUD'. The interface should be platform agnostic and must integrate seamlessly to web interfaces, reporting tools such as Tableau or data custom data platforms

My current project is to build a collection of restful that can be consumed by above mentioned platforms.

Architecture Decisions
---
* One monolithic application over microservices.
* Test strategy to impolement unit and integration tests.
* User management.
* Entity relationship management.
* A CI/CD pipeline to consume deployment triggers.

Tech Decisions
---
* Microservices to logically group the REST services and enable isolated deployment of these endpoints.
* Pytest framework to implement unit testing and integration testing.
* Auth0 to manage usermanagement of the application.
* Python's SQL alchemy to manage entity relationships
* Azure DevOps/Bitbucket Pipelines for building CI/CD pipeleine.


<!-- {{< figure src="/images/api-1.png" >}}
{{< figure src="/images/api-2.png" >}}
{{< figure src="/images/api-3.png" >}}
{{< figure src="/images/api-4.png" >}}
{{< figure src="/images/api-5.png" >}}
{{< figure src="/images/api-6.png" >}}
{{< figure src="/images/api-7.png" >}} -->

[Link to the api repository](https://github.com/chatter19/one_api_for_all)