---
date: 2020-06-10T11:00:59-04:00
description: "A ball classifier to identify balls from different sports."
featured_image: "/images/parser.png"
title: "Extract, Transform and Load: Parsing EDI Claims"
---
In order to improve the data ingestion strategies, I engineered a client agnostic data parser 
* extracts information from industry standard EDI (Electronic data interchange) files
* load data to the corresponding client databases
* run transformations (calculations) on the extracted data

Architecture Decisions
---
* a pluggable engine that is slient agnostic and cloud provider agnostic
* Implements a robust secret management paradigm
* Integrates with workflow management platforms such as Apache airflow
* A CI/CD pipeline to consume deployment triggers.

Tech Decisions
---
* Develop a pypi package for the parser
* Leveraged azure keyvaults and AWS Secret manager to manage client secrets
* Pytest framework to implement unit testing and integration testing.
* Azure DevOps/Bitbucket Pipelines for building CI/CD pipeleine.

Additional Features
---
* Documaentation integrated with codebase using Sphinx
* Custom logging on Application insights
* Automated PR review using Codeflow

<!-- {{< figure src="/images/parser.png" >}} -->

<!-- [Link to GitHub Repository](https://github.com/PlayingNumbers/ds_salary_proj) -->