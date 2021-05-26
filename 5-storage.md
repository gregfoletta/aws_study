---
title: AWS Cloud Practicioner - Storage
author: Greg Foletta
date: 26/5/2021
---

# Instance and EBS Stores

## Instance Store

Block level storage is like a hard drive - addressed at the block level. An **instance store** provides temporary block-level storage for EC2 instances. It's disk storage that's physically attached to the host of an EC2 instance, and has the same lifespan as the instance.

When the instance is terminated, the data is lost in the store.

## Elastic Block Store

EBS is a service that provides block level storage volumes to be used with EC2 instances. If an EC2 instance is stopped, all the data remains available. The storage is stored in a **single** availability zone.

You provision the storage, then attach it to the EC2 instance.

You can take incremental snapshops of the EBS volumes to back up the data.

# S3

Simple storage service - an object store where files are stored in buckets. Maximum size that can be uploaded is **5 Terabytes**. Versioning is also available.

Multiple buckets can be created with different classes or tiers (and thus costs) of data storage. Permissions  are assigned to limit who can see or access the objects.

## Storage Classes

- Standard
    - Frequently accessed data
    - Stored in a minimum of 3 AZs
- Standard-Infrequent
    - Similar to standard, but lower storage price and higher retrieval price.
- One-Zone Infrequent Access
    - Single AZ
    - Lower storage price and Standard.
    - Use if you can easily reproduce the data in the event of an AZ failure.
- Intelligent-Tiering
    - Data with unknown of changing access patterns
    - Monitors access patterns, if an object hasn't been accessed for 30 days, automatically moves it to the infrequent access tier.
    - If it gets accessed there, it's moved back.
    - Small monthly monitoring and automation fee per object
- Glacier
    - Low cost
    - Retrieve in minutes to hours
- Glacier Deep Archive
    - Lowest cost
    - Retreive within 12 hours

# EBS vs S3

- S3 already web enabled
- Every object has a URI and access rights
- Regionally distributed
- Object storage: every change needs a re-upload
- Complex reads and writes are better suited to EBS

# Elastic File System (EFS)

EFS is a managed, scalable file system, a regional resource. Grows and shrinks automatically. 

# RDS

A relational database, use SQL to query. Offers encryption at rest and encryption at transit.

Six database engines:

- Amazon Aurora
    - Compatible with PostgreSQL and MySQL
    - "5 times fast than MySQL and 3 x faster than PostgreSQL"
    - Reduce DB costs by reducing unnecessary I/O.
    - HA: replicates six copies of the data across three AZs
- PostgreSQL
- MySQL
- MariaDB
- Oracle Database
- Microsfot SQL Server

# DynamoDB

This is a non-relational DB - or "NoSQL". They use structures other than rows and columns to organise data. This could be key-value pairs. 10 trillion requests per day.

# RDS vs DynamoDB

RDS, with its strong structure, is suited to complex joins and analytics.

For anything else that doesn't have a relational structure you can use DynamoDB. Sometimes all people need is a lookup table. The NoSQL database is suited to this.

# Redshift

Data warehousing service that can be used for big data analytics. Collect data from many sources and understand relationships between them.

Issues that need to be solved:

- "Show me all production data" - data doesn't stop being ingested.
- Different data stores from different sources. Single query against multiple databases is difficult.

Once data becomes too complicated for relational DBs, you've entered the world of data warehousing.

With in coordination with **Spectrum**, Redshift can run a single query against exabytes of unstructured data.

# Migration Servicei (DMS)

Move between source and target databases. Can do relational, non-relational, and other types.

Other uses:

- Enable developers to test applications against production data.
- Combine several databases into a single database.
- Send ongoing copies of your data to other target sources instead of a one-time migration.

# Additional DB Services

- DocumentDB is a document database that supports MongoDB
- Neptune is a graph database, for apps with highly connected datasets.
- Quantum Ledger DB is a ledger DB, to review a complete history of all the changes made to your application data.
- Managed Blockchain is a service to create and manage blockchain networks with open-source frameworks.
- Elasticache adds caching layers on top of DBs using two types of data stores: Redis and Memcached.
- DynamoDB Accelerator (DAX) is an in-memory cache for DynamoDB. Improve response times from single-digit milliseconds to microseconds.




