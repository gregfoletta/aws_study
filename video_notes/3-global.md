---
title: AWS Cloud Practicioner - Global Infrastructure
author: Greg Foletta
date: 25/5/2021
---

# Regions

Data centres are built in regions. Inside each region there are multiple data centres. Each region can be connected to each other region through a high-speed fibre network controlled by AWS.

No data goes in our out of an environment in a region without permission being granted - regional data soverignty.

Proximity to your customers is a major factor in determining your region.

Four key factors:

- Compliance
- Proximity
- Feature availability
- Pricing


# Availability Zones

AWS calls a single data centre or a group of data centres an *availability zone* or **AZ**. Each as is one or more discrete data centres within a region.

Many AWS services run at the region level, so they run synchronously across multiple AZs without effort - an example is an ELB


# Edge Locations

An **edge location** is a site that CloudFront uses to store cached copies of your content closer to customers.

# Provisioning

There are multiple ways to interact with AWS however they are all backer by an API call:

- Management console 
    - Web based
- CLI interface
- Software Development Kits
- ElasticBeanStalk
    - Service that helps provision EC2 based environments.
    - Provide application code and desired configurations
    - Adjust capacity
    - Load balancing
    - Automatic scaling
    - Application health monitoring
- CloudFormation
    - Infrastructure as Code
    - Declarative format
    - Repeatable



There are other ways as well, including Elastic BeanStalk and CloudFormation


