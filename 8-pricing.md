---
title: AWS Cloud Practicioner - Pricing
author: Greg Foletta
date: 7/7/2021
---

# Free Tier

Enables you to begin using certain services without having to worry about incurring costs. There are three types:

- Always free: do not expire and are available to all AWS customers.
- 12 months free: free for 12 months following your initial sign-up date to AWS. 
- Trial: short-term free tiral offers from the date you activate a particular service.

# Pricing Concepts

Tnere are a range of services with pay-as-you-go pricing.

- Pay for what you use: for each service, pay for exactly the amount of resources you use.
- Pay less when you reserve: some services offer reservation options that provide significant discount compared to on-demand instance pricing.
- Pay less with volume based discounts: some services offer tiered pricing, so the per-unit cost is incrementally lower with increased usage.

# Pricing Calculator

The pricing calculator lets you explore AWS services and create and estimate for the cost of your use cases on AWS.

# Pricing Examples

## AWS Lambda

You're charged based on tkhe number of requests for your functions and the time it takes for them to run.

Allows 1 million free requests and up to 3.2 million seconds of compute time per month.

You can save by signing up for a compute savings plans.

## EC2

You pay for the compute time you use. You can use spot instances to reduce cost.

## S3

For S3 you consider the following cost components:

- Storage: you pay for the storage that you use, and you're changed the rate to store objects based on the sizes, storage classes, and how long the object is stored.
- Requestsyou pay for requests made to your S3 buckets.
- Data transfer: there is no cost to transfer between S3 and AWS services, however you need to pay for data into and out of S3, with some small exceptions.
- Management and Replication: you pay for the storage management features that you have enabled on you S3 buckets, like inventory, analytics and object tagging.

# Billing Dashboards

Use this to pay your bill, monitor usage, and analyse and control costs.

- Compare current month-to-date with the previous month
- View month-to-date spend by service
- View free tier usage by service
- Access cost explorer and create budgets
- Purchae and manage savings plans
- Publish cost and usage reports

# Consolidated Billing

AWS Organisations (discussed previously) provide the option for consolidated billing.

It enabled you to receive a single bill for all AWS accounts in your organisation. The default maximum number of accounts is 4, but this can be increased.

A benefit is that you can share bulk discount pricing, savings plans, and reserved instances across the accounts in the organisation.

# AWS Budgets

Create budgets to plan your service usage, service costs, and instance reservations.

Updates three times per day. Can set custom alerts when usage exceeds - or is forecasted to exceed - the budgeted amount.

# Cost Explorer

A tool that enabled you to visualise, understand, and manage costs over time.

Includes a default report that includes the costs and usage for your top five cost-accruing AWS services.

# Support Plans

There are four difference support plans to help you troubleshoot issues, lower costs, and efficiently use AWS services.

## Basic Support

Free to all customers, and includes whitepapers, documentation, and support communities.

You have access to a limited selection of AWS **Trusted Advisor** checks. You can use the **Personal Health Dashboard** tool that provides alerts and remediation guidance when AWS is experiencing events that may affect you.

## Developer Support

Access to:

- Best practice guidance
- Client-side diagnostic tools
- Building-block architecture support.

## Business Support

Have access to additional features including:

- Use-case guidance to identify AWS offerings, features, and services that can best support your specific needs.
- All AWS **Trusted Advisor** checks.
- Limited support for 3rd party software, such as common OSs and applicaton stack components.

## Enterprise Support

In addition to all the features of the other three plans, you also get

- Application architechture guidance, which is a consultative relationship.
- Infrastructure event management, a short term engagement with AWS support to understand your use cases.
- A **Technical Account Manager (TAM)**.

# Marketplace

A digital catalog that includes thousands of software listings from independent software vendors. Categories include:

- Business Apps
- Data and Analytics
- DevOps
- Infrastructure Software
- Internet of Things
- Machine Learning
- Migration
- Security.
