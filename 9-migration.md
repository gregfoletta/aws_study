---
title: AWS Cloud Practioner Essentials - Migration and Innovation
author: Greg Foletta
date: 8/6/2021
---

# Cloud Adoption Framework

The CAF organises guidnace into six areas of focus caled **'Perspectives'**:

## Business

The business perspective ensures IT aligns with business needs and it links to key business results.
 Use this perspective to create a strong business case for cloud adoption and prioritise cloud adoption initiatives.

Common roles:

- Business managers
- Finance managers
- Budget owners
- Strategy stakeholders

## People

Supports developerment of an *organisation-wise* change management strategy for cloud adoption.

Use this perspective to evaluate organisational structures and roles, new skill and process requirements, and identify gaps. This helps with staffing and training.

Common roles:

- Human resources
- Staffing
- People managers

## Governance

Focuses on the skills and processes to align IT strategy with business strategy. It ensures that business value is maximised, and risks and minimised.

Use this to understand how to update staff skills and processes, manage and measure cloud investments, and to evaluate business outcomes.

Common roles:

- Chief Information Officer (CIO)
- Program managers
- Enterprise architects
- Business analysts
- Portfolio managers

## Platform

Includes principles and patterns for implementing new solutions on the cloud, and migrating on-premises workloads to the cloud.

Use a variety of architectural models to understand and communicate the structure of IT systems and their relationships.

Common roles:

- Chief Technology Officer (CTO)
- IT managers
- Solutions architects

## Security

Ensures that the organisation meets the security objectives for visibility, auditability, and agility.

The CAF is used to structure the selection and implementation of security controls that meet the organisation's needs.

Common roles:

- Chief Information Security Officer (CISO)
- IT security managers
- IT security analysts

## Operations

Helps you enable, run, use, operate and recover IT workloads to the level agreed upon with your business stakeholders.

Common roles

- IT operations managers
- IT support managers

# Migration Strategies

There are six commons strategies when migrating to the cloud:

## Rehosting

This is the "lift-and-shift" model, which involves moving applications without changes.

## Replatforming

This is the "lift, tinker, shift", it involves making a few cloud optimisations to realise a tangible benefit. The optimisation does not change the core architecture of the application.

## Refactoring / Rearchitecting

Involves reimagining how an application is architectured and developed using cloud native features. Driving by a strong business need to add features, scale, or performance that would otherwise be difficult in the applications existing environment.

## Repurchasing

This involves moving from a traditional license to a software-as-a-service model.

## Retaining

This consists of keeping the core business applications in the existing environment.

## Retiring

Removing applications that are no longer needed.

# Snow Family

These are a family of devices that help to physically transport data into and out of AWS.

## Snowcone

is a small, rugged, secure edge computing and data transfer device. Features 2 CPUs, 4GB of memory, and 8TB of usable storage.

## Snowball

Offers two types of devices

- **Edge Storage Optimised** devices are well suited for large-scale data migrations. 80TB of HDD for block volumes and Amazon S3 object storage, and 1TB of SATA solid state. It also 40 vCPUs and 80GiB of memory to support Amazon sbe1 instances (equivalent of C5).

**Edge Compute Optimised** has 42TB of usable HDD and 7.68 TB of SSD. Has 52 vCPUs, 208GiB of memory, and an optional GPU. Can run sbe-c and sbe-g instances, equivalent to C5, M5a, G3 and P3 instances.

## Snowmobile

An exabyte-scale data transfer service used to move large amounts of data into AWS. Transfer up to 100 petabytes of data in a 45 foot ruggedised shipping container, pulled by a semi.

# Innovation

Need to focus on desired outcomes. Need to be able to articulate:

- Current state
- Desired state
- Problems you are trying to solve

Some paths that you might take:

## Serverless Applications

Don't require you to provision, maintain or administer servers.

## Artificial Intelligence

A variety of services are offered by AWS, for example:

- Speech to text with **Transcribe**
- Patters in text with **Comprehend**
- Identification of fraudulent online activities with **Fraud Detector**
- Voice and text chatbotswith **Lex**

## Machine Learning

AWS offers **SageMaker** to remove some of the difficult work from the process.


