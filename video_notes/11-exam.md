---
title: AWS Cloud Practicioner - Exam
author: Greg Foletta
date: 21/6/2021
---

# Exam Review

There are four domains:

- Cloud concepts
- Security and Compliance
- Technology
- Billing and Pricing


# Content


- Domain 1:Cloud Concepts
	- Define the AWS Cloud and its value proposition 
		-Define the benefits of the AWS cloud including:oSecurityoReliabilityoHigh AvailabilityoElasticityoAgility oPay-as-you go pricingoScalability oGlobal ReachoEconomy of scale
		-Explain how the AWS cloud allows users to focus on business valueoShifting technical resources to revenue-generating activities as opposed to managing infrastructure
	- Identify aspects of AWS Cloud economics
		-Define items that would be part of a Total Cost of Ownership proposaloUnderstand the role of operational expenses (OpEx) oUnderstand the role of capital expenses (CapEx)oUnderstand labor costs associated with on-premises operationsoUnderstand the impact ofsoftware licensing costs when moving to the cloud
		-Identify which operations will reduce costs by moving to the cloudoRight-sized infrastructureoBenefits of automation oReduce compliance scope (for example, reporting)oManaged services (for example, RDS, ECS, EKS, DynamoDB)
	- Explain the different cloud architecture design principles
		-Explain the design principlesoDesign for failureoDecouple components versus monolithic architectureoImplement elasticity in the cloud versus on-premisesoThink parallel
- Domain 2:Security and Compliance
	- Define the AWS shared responsibility model
		-Recognize the elements of the Shared Responsibility Model 
		-Describe the customer’s responsibly on AWSoDescribe how the customer’s responsibilities may shift depending on the service used (for example with RDS, Lambda, or EC2)
		-Describe AWS responsibilities
	- Define AWS Cloud security and compliance concepts
		-Identify where to find AWS compliance informationoLocations of lists of recognized available compliance controls (for example, HIPPA, SOCs)oRecognize that compliance requirements vary among AWS services
		-At a high level, describe how customers achieve compliance on AWSoIdentify different encryption options on AWS (for example, In transit, At rest)
		-Describe who enables encryption onAWS for a given service
		-Recognize there are services that will aid in auditing and reportingoRecognize that logs exist for auditing and monitoring (do not have to understand the logs)oDefine Amazon CloudWatch, AWS Config, and AWS CloudTrail
		-Explain the concept of least privileged access
	- Identify AWS access management capabilities
		-Understand the purpose of User and Identity Management oAccess keys and password policies (rotation, complexity)oMulti-Factor Authentication (MFA)oAWS Identity and Access Management (IAM)•Groups/users•Roles•Policies, managed policies compared to custom policiesoTasks that require use of root accountsProtection of root accounts
	- Identify resources for security support
		-Recognize there are different network security capabilitiesoNative AWS services (for example, security groups, Network ACLs, AWS WAF)o3rdparty security products from the AWS Marketplace
		-Recognize there is documentation and where to find it (for example, best practices, whitepapers, official documents)oAWS Knowledge Center, Security Center, security forum, and security blogsoPartner Systems Integrators
		-Know that security checks are a component of AWS Trusted Advisor
- Domain 3: Technology
	- Define methods of deploying and operating in the AWS Cloud 
		-Identify at a high level different ways of provisioning and operating in the AWS cloudoProgrammatic access, APIs, SDKs,AWS Management Console, CLI, Infrastructure as Code
		-Identify different types of cloud deployment modelsoAll in with cloud/cloud nativeoHybridoOn-premises
		-Identify connectivity optionsoVPNoAWS Direct ConnectoPublic internet
	- Define the AWS global infrastructure
		-Describe the relationships among Regions, Availability Zones, and Edge Locations
		-Describe how to achieve high availability through the use of multiple Availability ZonesoRecall that high availability is achieved by using multiple Availability ZonesoRecognize that Availability Zones do not share single points of failure
		-Describe when to consider the use of multiple AWS RegionsoDisaster recovery/business continuityoLow latency for end-usersoData sovereignty
		-Describe at a high level the benefits of Edge LocationsoAmazon CloudFrontoAWS Global Accelerator
	- Identify the core AWS services
		-Describe the categories of services on AWS (compute, storage, network, database)
		-Identify AWS compute servicesoRecognize there are different compute familiesoRecognizethe different services that provide compute (for example, AWS Lambda compared to Amazon Elastic Container Service (Amazon ECS), or Amazon EC2, etc.)oRecognize that elasticity is achieved through Auto ScalingoIdentify the purpose of load balancers
		-Identify different AWS storage servicesoDescribe Amazon S3oDescribe Amazon Elastic Block Store (Amazon EBS)oDescribe Amazon S3 GlacieroDescribe AWSSnowballoDescribe Amazon Elastic File System (Amazon EFS)oDescribe AWS Storage GatewayoIdentify AWS networking servicesoIdentify VPCoIdentify security groupsoIdentify the purpose of Amazon Route 53oIdentify VPN, AWS Direct Connect•Identify different AWS database servicesoInstall databases on Amazon EC2 compared to AWS managed databaseso
	Identify Amazon RDSoIdentify Amazon DynamoDBoIdentify Amazon Redshift
	-Identify resources for technology support 
		-Recognize there is documentation (best practices, whitepapers, AWS Knowledge Center, forums, blogs)
		-Identify the various levels and scope of AWS supportoAWS AbuseoAWS support casesoPremium supportoTechnical Account Managers
		-Recognize there is a partner network (marketplace, third-party) includingIndependent Software Vendors and System Integrators
		-Identify sources of AWS technical assistance and knowledge including professional services, solution architects, training and certification, and the Amazon Partner Network
		-Identify the benefits of using AWS Trusted Advisor
- Domain 4: Billing and Pricing
	- Compare and contrast the various pricing models for AWS (for example, On-DemandInstances, ReservedInstances,and Spot Instancepricing)
		-Identify scenarios/best fit for On-Demand Instance pricing
		-Identify scenarios/best fit for Reserved-Instance pricingoDescribe Reserved-Instances flexibilityoDescribe Reserved-Instances behavior in AWS Organizations
		-Identify scenarios/best fit for Spot Instance pricing
	- Recognize the various account structures in relation to AWS billing and pricing
		-Recognize that consolidated billing is a feature of AWS Organizations
		-Identify how multiple accounts aid in allocating costs across departments
	- Identify resources available for billing support
		-Identify ways to get billing support and informationoCost Explorer, AWS Cost and Usage Report, Amazon QuickSight, third-party partners, and AWS Marketplace toolsoOpen a billing support caseoThe role of the Concierge for AWS Enterprise Support Plan customers
		-Identify where to find pricing information on AWS servicesoAWS Simple Monthly CalculatoroAWS Services product pagesoAWS Pricing API
		-Recognize that alarms/alerts exist
		-Identify how tags are used in cost allocation



