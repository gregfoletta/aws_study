---
title: AWS Cloud Practicioner - Compute
author: Greg Foletta
date: 24/5/2021
---


EC2 is highly flexible, cost effective and quick. With on-prem, you have to purcase hardware up-front, wait until they're delivered, rack and stack. Once you buy the servers, you're stuck with them.

- AWS built data centres
- AWS secured data centres
- AWS purchased servers
- AWS installed servers
- Servers are online and ready to be used.

You only pay for running instances, not stopped instances.

You can veritcally scale an instance by giving it more CPU and more memory.


# How EC2 Works

- Launch an instance by selecting a template with basic configuration.
- Connect - connect the instance.
- Use

# Instance Types

- General purpose instances have a balance of compute, memory and networking resources.
- Compute optimised instances are good for compute-intensive tasks like gaming, HPC and scientific modelling.
- Memory optimised are good for memory-intensive tasks.
- Accelerated compute are good for floating point / graphics. These have hardware accelerators or coprocessors to perform some functions more efficiently.
- Storage optimised are good for high-performance locally stored data

# Pricing

- On-Demand - only pay for the duration the instance runs for.
    - Per-hour or per-second.
    - Short-term, irregular workloads that cannot be interrupted.
- Savings - low prices on EC2 in exchange for a commitment to a consistent amount of usage measured in dollar per hour. Save up to 72% on AWS compute usage.
    - Also applies to AWS lambda
    - 1 year or 3 year terms
- Reserved - suited for steady state workloads
    - Offer up to 75% discount
    - 1 or 3 year term.
- Spot - request spare EC2 computing capacity for up to 90% of the on-demand price.
    - AWS can reclaim the instance at any time they need it, giving you a two-minute warning.
    - Ideal for workloads with flexible start and end times.
    - Up to 90% discount on on-demand costs.
- Dedicated - physical hosts dedicated for your use.


# Scalability

Beginning with the resources you need, and designing the architecture to automatically respond to changing demand.

The funcitionality for EC2 instances is **Amazon EC2 Auto Scaling**.

Two approaches:

- **Dynamic scaling**: responds to changing demand
    - **Minimum**: Set the minimum number of EC2 instances
    - **Desired**: Create an auto scaling group, set the minimum number of EC2 instances that launch immediately.
    - **Maximum**: Set the desired capacity.
- **Predictive scaling**: automatically schedules the right numnber of instances based on predicted demand.

# Elastic Load Balancing

ELB distributes incoming application traffic across multiple EC2 instances. Separate to EC2, but they work together to help ensure applications have high availability and performance.

# Messaging and Queuing

In a microservices approach, components are loosely coupled. When designing AWS apps, two services facilitate integration of microservices: SNS (Simple Notification Service) and SQS (Simple Queueing Service).

## SNS 

Is a pub/sub service. Using topics, a publisher publisher messages to subscribers. In SNS the subcribers can be web servers, email addresses, lambda functions, or other options.

## SQS

In SQS, you can send, store, and receive messages between software components without losing messages or requiring other services to be available. An application sends a message to a queue. A user or service retrieves a message from the queue, processes it, then deletes it from the queue.

# Lambda

Is a service that lets you run code without needing to provision or manage servers. You pay for the compute time you use, while the code is running. Works as follows:

- Upload code
- Set code to trigger from an event source
- Code runs only when triggered
- Pay for the compute time you use

# Elastic Container Service

Containers are a standard way to package application code and dependencies in a single object. ECS is a container management system that enables you to run and scale containerised applications.

Supports Docker containers. Youj use API calls to lauch and stop Docker-enabled applications.

# Elastic Kubernetes Service 

Fully manages service running Kubernetes on AWS. This allows you to deploy and manage containerized applications at scale.

# Fargate

Serverless compute engine for containers. Works with both ECS and EKS. You don't need to provision or manage servers.


