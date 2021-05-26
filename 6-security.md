---
title: AWS Cloud Practitioner Essentials - Security
author: Greg Foletta
date: 27/5/2021 
---

The **shared responsibility model** is a construct whereby AWS controls the security *of* the cloud and customers control the security *in* the cloud.
 
# Shared Responsibility Model

AWS is responsibile for:

- Regions, Zones and Edge locations
- Hardware and Global Infra
- Compute, Storage, Database and Networking
- Software

Customer is responsible for:

- Client-Side Data encryption
- Server-Side encryption
- Network traffic protection
- Operating systems, network and firewall config
- Platform, applications, identity and access management
- Customer data


# User Permissions

Identity and Access Management (IAM) manages the access to AWS services and resources.


## Root User

When an AWS accout is created, you begin with a root user. It has complete access to all resources. You should not use this user for everyday tasks.

## IAM Users

These are identities created in AWS. It represents a person or application that interacts with AWS services and resources. It consists of a name and credantials.

New users have no permsissions.

## IAM Policies

An IAM policy is a document that allows or denies permissions to AWS services and resources.

Should follow the principle of *least privilege* when granting permissions.

## IAM Groups

An IAM grou
.
