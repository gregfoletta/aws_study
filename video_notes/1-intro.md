---
title: AWS Cloud Practictioner - Intro
author: Greg Foletta
date: 21/5/2021
---


# Cloud Compute

- Client server models.
- Amazon Elastic Compute Cloud (EC2)
- **Key Concept**: only pay for what you use, first key value

## Deployment Models

Companies must consider different factors when determining a cloud strategy:

- Cloud components
- Resource management tools
- Legacy IT infra requirements.

Three models:

### Cloud Based Deployment

- Everything in the cloud
- Migrate existing applications to the cloud
- Design and build new apps in the cloud

### On-Premises Deployment

- Deploy resources by using virtulisation and resource management tools
- Increase utilisation by using applications management and virtulisation technologies.
- Also known as "private cloud".

### Hybrid Deployment

- Conect cloud-based resources to on-premises infra.
- Integrate cloud based resources with legacy IT applications.

Can be usefuly in situations where there are legacy applications, or government regulations that mean you can't move apps to the cloud.

## Cloud Benefits

- Trade upfront expense for variable expense.
- Reduce spend on maintaining data centres
- No need to guess capacity - spin up when you need it.
- Benefit from economies of scale that AWS brings
- Increase speed and agility - the flexibility if cloud makes it easier to develop and deploy applications
- Global footprint.

## AWS Overview PDF

[Located Here](https://d0.awsstatic.com/whitepapers/aws-overview.pdf)

### Cloud Computing Models

**Iaas** contains the basic building blocks, and typically provides access to networking, compute, and storage.

**PaaS** removes the need to manage the underlying infrastructure (hardware and OS) and allows you to focus on the deployment and management of your applications.

**SaaS** provides a completed product that is run and manages by the service provider. You don't have to think about how it's hosted or maintained, only how you use that piece of software.

### Analytics

**Athena** is an interactive query service, allowing you to analyse data in Amazon S3 using standard SQL. Pay for the queries that are run. Integrated with AWS Glue Data Catalog.

**EMR (Elastic MapReduce)** provides a managed Hadoop framework allowing you to process data across dynamically scalable EC2 instances. Can also run Apache Spark, HBAse, Presto, and Flink, and interact with data in S3 and DynamoDB.

**CloudSearch** a search solution for websites, 34 languages, autocomplete, geospatial search.

**Elasticsearch** allows you to deploy and operate Elasticsearch to analyze and visualise data in real-time. USe for log analytics, full-text search, application monitoring, clickstream analytics. Integrate with Kibana and Logtash.

**Kinesis**: collect, process and analyze real-time streaming data. Inest video, audio, application logs, clickstream, IoT telemetry data. Process the data as it arrives. Comes in four flavours: *Data Firehose, Data Analytics, Data Streams* and *Video Streams*.

**Redshift**: data warehousing. Parallel queries and columnar storage on high performance disk.

**Quicksight** business intelligence tool. Publish interactive dashboards.

**Data Pipeline**: a web service to move data between different AWS compute and storage services, as well as on-prem data sources, at specified intervals. Integrates with S3, RDS, DynamoDB and EMR.

**Glue**: extract, transform and load (ETL) service. Prepare and load your data for analytics.

**Lake FOrmation**: a data lake. Centralised, secured and curated repository of all data, both original and transformed/cleaned. Break down into silos, combine different analytics.

**Manaed Streaming for Apache Kafka (MSK)**: use Apache Kafka APIs to populate data lakes, stream changes to a from DBs.

### Applications Integration

**Step Functions**: coordinate multiple AWS services into serverless workflows.

**MQ**: managed message broker service for Apache ActiveMQ. Allows different software systems to communicate and exchange information.

**SQS**: simple query service. Decouple microservices, distributed systems and serverless applications.

**SNS**: notification service, pub/sub messaging. Can be used to fan out notifications to end users as well using mobile push, SMS and email.

**SWF**: simple workflow, build and run background jobs that have parallel or sequential steps.

### AR and VR

**Sumerian**: run VR, AR and 3D applications.

### Cost Management

**Cost Explorer**: visualise, understand and manage AWS costs.

**Budgets**: set custom budgets that alert when costs are exceeded.

**Cost Usage and Report**: access comprehensive information about your AWS costs and usage.

**Reserved Instance Reporting**: RI specific cost management solution.

### Blockchain

**Managed Blockchain**: create and manage scalable blockchain networks using open source frameworks like *Hyperledger Fabric* and *Ethereum*.

### Business Applications

**Alexa for Business**: use Amazon Alexa in a business scenario.

**WorkDocs**: enterprise storage and sharing service.

**WorkMail**: managed business email and calendar service.

**Chime**: communications service and online meetings. Works with Alexa for business.

### Compute Services

**EC2**: elastic cloud compute.

**Elastic Container Registry**: fully managed docker container registry, integrated with the elastic container service.

**Elastic Container Service**: container orchestration service that supports Docekr containers.

**Elastic Kubernetes Service**: deploy, manage and scale applications using Kubernetes.

**Lightsail**: easy way to set up and launch a private server. Includes SSD storage, data trasfer, DNS, static IP.

**AWS Batch**: run batch jobs on AWS. Plans, schedules and runs the jobs across the full range of AWS compute services.

**Elastic Beanstalk**: service for deploying web applications and services developed with Java, .NET, PHP, Node.JS, Python, Ruby, Go, and Docker on servers such as Apache, NGNIX, Passenger and IIS.

**Fargate**: run containers without having to manage servers or clusters.

**Lambda** run code without provisioning or managing servers. 

**Serverless Application Repository**: deploy code samples, componenets and complete applications for common use cases. 

**Outposts**: bring native AWS servers, infrastructure and operating models to any data centre, colo on on-prem facilty. Comes in a VMWare cloud or AWS native.

**VMWare Cloud on AWS**: join cloud offering that allows you to extend your on-premises VMWare vSphere environment to the AWS cloud.

### Customer Engagement

**Connect**: self-service, cloud based contact center service.

**Simple Email Service (SES)**: cloud based email sending service.

### Database

**Aurora**: MySQL and PostgreSQL compatible relational database engine.

**Relational Database Service (RDS)**: Relational database in the cloud. Six different database engines: Aurora, PostgreSQL, MySQL, MariaDB, Oracle and SQL Server.

**RDS on VMWare**: deploy managed databases on in-premises VMWare environments using RDS technology.

**DynamoDB**: key-value and document database.

**ElastiCache**: web serverice in-memory cache in the cloud. Supports Redis and Memcached.

**Neptune**:  graph database service. Suppors graph models *Property Graph* and *RDF*.

**Quantum Ledger Database (QLDB)**: ledger database that provides a transparent, immutable and cryptographically verifiable transaction log.

**Timestream**: time series database for IoT and operational applications.

**DocumentDB**: document database service that supports MongoDB workloads.

### Desktop and App Streaming

**WorkSpaces**: cloud desktop service, supporting Linux and Windows.

**AppStream 2.0**: application streaming service.

### Developer Tools

**CodeCommit**: source control service based on Git repositories.

**CodeBuild**: fully managed build service that compiles, runs tests, and produced software packages.

**CodeDeploy**: automates code deployments to any instance, including EC2 and those running on-prem.

**CodePipeline**: continuous delivery service, automating release pipelines.

**CodeStar**: develop, build and deploy applications in AWS. Unified user interface enabling you to manage your software development activities in one place.

**Corretto**: no-cost, multiplatform distribution of the Open Java Development Kit (OpenJDK).

**Cloud9**: cloud-based integrated development environment in the browser.

**X-Ray**: analyse, and debug distributed applications. End-to-end view of requests as they travel through an application.

### Game Tech

**GameLift**: managed service for deploying, operating, and scaling dedicted game servers.

**Lumberyard**: cross-platform game engine.

### IoT

**IoT Core**: managed cloud service that lets connected devices interact with cloud applications.

**FreeRTOS**: operating system for microcontrollers that makes small, low-power edge devices easy to program.

**IoT Greengrass**: Extends AWS to devices so they can act locally on the data they generate, while still using the cloud for management, analytics and durable storage. Can run Lambda functions, execute predictions based on ML models even when not connected to the internet.

**IoT 1-Click**: Enables simple devices to trigger lambda functions.

**IoT Analytics**: a service that allows you to run and operationalise sophisticated analytics on massive volumes of IoT data. It filters, transforms and enriches that IoT data before storing it in a time series database.

**IoT Button**: programmable button based on the Amazon Dash Button hardware.

**IoT Device Defender**: secure your fleet of IoT devices. Audits your IoT configurations to make sure they aren't deviating from security 'best practices'.

**IoT Device Management**: on-board organise, monitor and remotely manage IoT devices at scale.

**IoT Events**: detect and respond to events coming from IoT sensors.

**IoT SiteWise**: collect, store, organise and monitor data from idustrial equipment.

**IoT Things Graph**: visually connect different devices and web services to build IoT applications.


### Networking and Content Delivery

**VPC**: virtual private cloud, provision a logically isolated section of the AWS cloud.

**CloudFront**: a fast content delivery network.

**Route 53**: cloud DNS web service.

**PrivateLink**: provides private connectivity between VPCs, AWS services, and on-premises applications.

**DirectConnet**: establish a dedicated network connection between your network and one of the AWS Direct Connect locations.

**Global Accelerator**: improves the availabilitY and performance of the applications that you offer to global users. It provides static IP addresses that act as fixed entry points.

**API Gateway**: create your an API thast acts as a front door for applications to access data, business logic or functionality.

**Transit Gateway**: connect VPCs and on-premises networks to a single gateway. You can connect pairs of VPCs using peering, however managing point-to-point connectivity is operationally cumbersome. With transit gateway, you create and manage a single connection from a central gateway in to each VPC, on-prem DC or remote office.

**App Mesh**: monitor and control microservices running on AWS.

**Cloud Map**: resource discovery service.

**Elastic Load Balancing**: distributes incoming application traffic across multiple targets, including EC2 instances, containters, and IP addresses.
