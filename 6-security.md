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

An IAM groups are a collection of IAM users, and to which you can assign IAM policy.

## IAM Roles

A role is an identity you can assume to gain temporary access to permissions. Before a user, application or service can assume an IAM role, they need to be granted permissions to switch to the role.

When they assume the role, they abandon all previous permissions they had under the previous role.

## Multi-factor Auth

MFA provides an extra layer of security. The factos could be a key fob, hardware device, or MFA app on a smart phone.

# AWS Organisations

If a company has multiple AWS accounts, AWS organisatons can consolidate and manage access to these from a central location.

In AWS Orgs, you can centrally control permissions for the accounts in your org by using **service control policies**. SCPs enable you to place restrictions on the AWS services, resources, and individual API actions that users and roles in each account can access.

## Organisational Units

OUs allow the grouping of accounts to make it easier to manage accounts with similar business or security requirements. When a policy is applied to an OU, all the accounts in the OU automatically inherit the permissions.

You can isolate workloads or applications that have specific security requirements.

SCPs can be applied to organisational units or to individual accounts.

# Compliance

Depending on the industry you may need to uphold certain security standards. **AWS Artifact** is a service that provides on-demand access to AWS security and compliance reports and online agreements. There are two main sections:

- AWS Artifact Agreements
    - Review, accept and manage agreements for an individual account and for all your accounts in AWS Organisations.
    - Different agreements are offered to address the needs of customers who are subject to specific regulations (e.g. HIPAA).
- AWS Artifact Reports
    - This gives you information on responsibilities for complying with certain regulatory standards.
    - Provides compliance reports from thirs party auditors.
    - These auditors have tested and verified that AWS is compliant with a variety of global, regional and industry-specific security standards.

## Customer Compliance Centre

Contains resources to help learn more about AWS compliance. There are:

- Compliance stories
- Whitepapaers
    - Answers to compliance questions
    - Overview of AWS risk and compliance
    - Auditing security checklists

# Denial of Service Attacks

A deliberate attempt to make a website or application unavailable to users. A distributed denial of service attack is where multuple sources are used to start an attack that aims to make a website or application unavailable.

**AWS Shield** is a service that protects applications against DDoS attacks. **Standard** autmatically protects all AWS customers at no cost. **Advanced** is a paid service that provides detailed attack diagnostics and the ability to detect and mitigate DDoS attacks. Integrates in with other services like CloudFront, Route53 and ELB. Can integrate in to AWS WAF by writing custom rules.

# Additional Security Services

## Key Management Service (KMS)

Enables encryption operations through the use of cryptographic keys.

## WAF

Web Application Firewall that monitors network requests coming in to web applications. Works with CloudFront and Application Load Balancer.

## Inspector

Helps improve the security and compliance of applications by running automated security assessments. Checks applications for security vulnerabilities and deviations from best practices. e.g open access to EC2 instances and installations of vulnerable software versions.

## GuardDuty

Intelligent threat detection for your AWS infrastructure and resources. Monitors network activity and account behaviour.

Analyses data from multiple sources:

- VPC flow flows,
- DNS logs

Review findings and look at recommended steps for remediation.

Lambda functions can be put in place for automatic response to findings.


