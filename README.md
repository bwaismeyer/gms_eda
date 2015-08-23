# Exploratory Data Analysis of Mass Shootings and the Gun Market
This document provides a summary of project goals, intended products, and 
relevant supporting information. 

## Acronyms
**MS-EDA**: Project shorthand.

## Project Motives
We want to better understand mass shootings and are curious about their
economic impact on the gun market. In other words, we are satisfying personal
curiousity and practicing data science skills for our own professional 
development.

## Project Objective
Explore the history of mass shootings in the US, the history of gun sales,
and assess if there is any relationship between the two.

## Project Goal
We want to provide easy-to-read visualizations and insights to inform 
conversations around mass shootings, gun sales, and any possible relationships
between the two.

All code and data should be captured as an R package so that it is documented
and reproducible.

## Audience Definition
Project data and write-ups will be tailored to a broad audience interested
in the topics of mass shootings and guns sales. Data will be made available in 
a broadly accessible format (e.g., CSV or Excel files) and at least some blog 
posts will be non-technical.

Project code will be tailored towards analysis-savvy people who are
comfortable with (or willing to learn) R.

## Key Tasks Product Will Support for Target Audience(s)
Our broader audience should be able to:
* Understand the premise of the study
* Observe broad trends and key takeaways
* Obtain the data in a non-specialized format

Analytically-minded folks should be able to:
* Access our finalized data as a built-in dataframe (or set of dataframes) in
    the same R package
* Access our code for gathering and cleaning data in the same R package
* Reproduce any analyses we complete or visualizations we produce either via
    documented R package functions or via clearly presented code in blog post

## Deliverables
1. R code for gathering and cleaning data (R package)
2. Finalized data in multiple formats (R package, CSV, Excel)
3. R code for analyses and visualizations (R package and/or blog posts)
4. Non-technical summary of demographics via blog post (R markdown)
5. Non-technical summary of other key observations via blog post (R markdown)
6. At least one technical dive into analysing shooting ~ sales relationships, 
    prepared as a well-structured R markdown file and knitted into a blog post

## Technical Requirements
All scraping and analysis should be completed in R or be executed by functions 
in the planned R package.

## Milestones
* Identify data targets, broad and narrow
* Identify data sources and match them to targets
* Shell and name for R package
* Plan and code strategies for gathering data
* Plan and code data cleaning
* EDA
* Plan and code demographics analysis and visualizations
* Prepare demographics blog post - non-technical but code available
* Plan and code any follow-up analyses, including success work
* Prepare technical version of follow-up post(s)
* Prepare non-technical version with key takeaways
* Finalize R package and documentation on GitHub

## Limits and Exclusions
This project may collect data for other incidents of mass violence, but will
limit analysis to mass shootings per the FBI definition (4 or more victims in
a relatively contained time).