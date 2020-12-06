---
date: 2017-04-10T11:00:59-04:00
description: "A ball classifier to identify balls from different sports."
featured_image: "/images/parser.png"
title: "Extract, Transform and Load: Parsing EDI Claims"
---

EDI or Electronic Data Interchange is a standard for a p2p exchange of business documents.

In this project, I created a parser that extracts PHI data from unstructured industry standard EDi files and generates a structured data format to be consumed by the downstream data pipeline

The parser has the following capabilities:
---

* Developed a custom utility to asynchronously read and parse millions of files using asyncio

* The parser is developed as a pluggable interface and can be integrated in any pipeline as a library

* Integrated the parser to work with the Azure cloud resources - Azure Keyvault/Blob/Azure data warehouse as well as with AWS resources (AWS secret manager/S3/Redshift database)
Leveraged pytest to achieve 100% integration testing on both cloud platforms

* Built document as code

* Automated PR review using Codeflow

* Implemented a CI/CD pipeline to continuously test new code commits


{{< figure src="/images/parser.png" >}}

<!-- [Link to GitHub Repository](https://github.com/PlayingNumbers/ds_salary_proj) -->