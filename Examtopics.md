https://www.examtopics.com/exams/amazon/aws-certified-cloud-practitioner-clf-c02/view/18/
last page for free access
finished review by 2024-01-16
test taken 20240-01-17

++++++++++++++++++
# S3
- data into S3 FREE, Data out of S3 NOT
- highly durable object storage
## Versioning
- preserve, retrieve, restore every version of every objects in S3

# Amazon FSx
- fully managed Windows file server

# AWS Storage Gateway
- hybrid storage service (connects on-prem with S3)
- provide on-prem access to virtually unlimited cloud storage
## AWS S3 File Gateway
- supports NFS and SMB
## AWS FSx File Gateway
- supports SMB only

# S3 Transfer Acceleration
- utilized Amazon CloudFront's globally distributed edge locations to accelerate object upload


++++++++++++++++++
# Amazon Macie
- automatically discover, classify and protect sensitive data
- fully managed data security and data privacy service
- uses ML and pattern matching to discover and protect sensitive data

# Amazon CloudFront
- web service that speeds up distribution of your static, dynamic web content
- content cached in edge locations

++++++++++++++++++
# Access Keys
- long-term credentials for an IAM user or AWS account root user
- use access keys to sign *programmatic requests to the AWS CLI or AWS API*

# Gain Programmatic Access
- Access Key ID
- Secret Access Key

++++++++++++++++++
# EC2
## Rightsizing 
- AWS Cost Explorer, AWS Compute Optimizer
## On-Demand Instances
- apps with short-term, spiky, unpredictable workloads 
- high abailability (downtime must be avoided)
## Reserved Instances
- capacity reservation (1 year)
- when traffic predictable, consistent
- discount up to 75%
## Saving Plans
- upfront commitment
- discount up to 72%
## Spot Instances
- for stateless, fault-tolerant workload
- no need to run at speific times

# EC2 Image Builder
- automate creation, maintain, validate, and test EC2 AMIs

++++++++++++++++++
# AWS Service Catalog
- deploy and govern as IaC templates

# AWS CloudFormation
- model, provision, manage AWS and third-party resources by treating IaC

# AWS CDK (Cloud Development Kit)
- software development framework
- provision resources through AWS CloudFormation

++++++++++++++++++
# AWS Cost Explorer
- visualize, manage spending and usage

# AWS Budget
- set custom cost and usage budgets
- trigger actions when threshold is reached

++++++++++++++++++
# AWS CloudWatch
- monitoring service used to collect metrics, logs, events from AWS resources
- supports setting up alerts
- i.e. w/ CloudTrail, motnitor and receive alerts about sign-in events

# AWS CloudTrail
- records all API calls made on your AWS account
- i.e. termination of EC2 instances

# AWS SNS (Simple Notification Service)
- sends text and email from distributed applications

# AWS Security Hub
- CSPM Service
- aggregates (security) alerts from various AWS service

++++++++++++++++++
# AWS Knowledge Center
- knowledge base of information

++++++++++++++++++
# Amazon Inspector
- for Vulnerability / Security Assessment
- automated vulnerability management services
- on applications deployed on EC2

# AWS Trusted Advisor
- Benefits:
  - Cost optimization, Performance, Security, Fault tolerance, Service quotas
- Checks security groups that allow unrestriced access to resources

# Amazon Config
- for Compliance
- continuously monitor and records changes of AWS resources

# AWS Professional Services
- consulting arm for migrating workloads on AWS

# AWS Elastic Beanstalk
- deploys app quickly, without manually creating resources

# AWS Health Dashboard
- centralized location for AWS service availability and operations

++++++++++++++++++
# AWS Glue
- serverless data integration service
- prepare and load data for analysis

# Amazon QuickSight
- business intelligence(BI) at hyperscale
- create and visualize interactive dashboards
- includes ML insights

# AWS Athena
- occasionally run queries for data analysis
- serverless query service 
- analyze data directly in Amazon S3 using standard SQL queries

# Amazon Redshift
- fully-managed data warehouse service

# Amazon Kinesis
- real-time processing of streaming data

# Amazon RDS
- managed relational database service
- running queries directly on data stored in S3
- most cost-effective
- supports various DB engines
  - PostgreSQL for OLTP workloads

# Amazon Aurora
- relational DB
- fully managed MySQL, PostgreSQL-compatible DB

# Amazon DynamoDB
- non-relational DB
- key-value dB
- sub-millisecond latency on a large scale
- shared responsibility modelx:
  - physical security, patching, encrypting

# Amaon DAX (DynamoDB Accelerator)
- reduce response time of DynamiDB table from milliseconds to microseconds

++++++++++++++++++
# CAF Capabilities and Perspectives
- BPS-GPO:
  - Business, People, Security, Governance, Platform, Operations
1. Business = Strategic Partnership
2. People = Cloud Fluency
3. Security = Threat Detection
4. Governance = Program & Project Management
5. Platform = Data Architecture
6. Operations = Event Management 
![CAF Capabilities](CLF-C02/CAF%20Capabilities.png)

# CAF Transformation Journey
1. Envision phase = domonstrating how cloud will help accelerate your business outcomes
2. Align phase = identifying capability gaps
3. Launch phase = delivering pilot initiatives
4. Scale phase = expanding production pilots and business value
![CAF Transformation](CLF-C02/CAF%20Transformation.png)

# AWS Well-Architected Framework
- OSR PC
1. Operational Excellence
2. Security
3. Reliability
  - Multiple AZs
4. Performance Efficiency
  - use computing resources efficiently to meet system requirements
5. Cost Optimization

# AWS
- Agility
  - provision and deprovision resource *rapidly*
  - Ability to experiment quickly
- Elasticity
  - Ability to rightsize resources as demand shifts
  - How easily resources can be procured when the are needed

# AWS Shared Responsibility Model
- full AWS
  - physical and environmental controls
  - security "of" the cloud infrastructure
- shared controls
  - patch management
  - configuration management (infra - AWS, OS & DB & Apps - Customer)
  - awareness & training
- full customer
  - service, communication protections, zone security
  - security "in" the cloud infrastructure
  - i.e. data transfer between S3 and on-prem apps

# AWS Benefits
- High economies of scale
- Launch globally in minutes

++++++++++++++++++
# AWS Consolidated Billing 
- one bill for multiple accounts
- combined usage, volume pricing discounts

++++++++++++++++++
# AWS Lambda
- charged by (1) run time (2) # of requests
- max run time 15mins

# AWS Fargate
- serverless compute for containers

++++++++++++++++++
# AWS Internet Gateway
- allow communication between VPC and Internet

# AWS Transit Gateway
- connects VPCs to on-prem networks through a central hub
- acts as a highly scalable cloud router

# Elastic Load Balancer
- acceps traffic from clients and routes to registered targets in one or more AZ
- does not accept targets across regions

# AWS Direct Connect
- dedicated network connection between on-prem and AWS
- no internet inbetween
- uses standard Ethernet fiber-optic cable

# AWS Connect
- omnichannel cloud contact center
- seamelss voice and chat service

# AWS Site-to-Site VPN
- encrypted network connection between on-prem and AWS
- uses internet

# AWS Client VPN
- a managed client-based VPN service
- uses OpenVPN

# Security Groups
- stateful firewalls
- control traffic at the instance level
- define types of network traffic

# Network ACLs (Access Control Lists)
- stateless firewalls
- control traffic at the subnet level
- define source, destination IP, ports

# VPC Flow Logs
- provide log information of inbound and outbound traffic on network interfaces in a VPC

++++++++++++++++++
# AWS WAF
- deals with common web attack patterns (XSS, SQL Injection, etc...)

# AWS Shiled
- deals with DDoS

# AWS Artifact
- a service to query for security related reports
- central resoruce for compliance-related information
- provides compliance reports

# AWS GuardDuty
- threat detection service
- monitor and detect potential security threats in AWS env.
- monitors misconfigured security groups

++++++++++++++++++
# AWS CodeArtifact
- a managed artifact repository service
- stores and shares sw that is ready for deployment

# AWS CodeBuild
- automatically compile source code, run unit tests, produce sw packages ready for deployment

# AWS CodePipeline
- manages movement of code between individual services

# AWS CodeCommit
- source code version control service
- helps user store and manage developer's source code in AWS

++++++++++++++++++
# Loosely Coupled Dependencies
- main advantage of moving from *monolithic to microservices*
- asynchronous communication and decouple components
- Amazon SQS (Simple Queue Service), AWS Step Functions

# Refactor
- or re-architect
- convert a monotholic application into microservices

++++++++++++++++++
# AWS IAM
## Credential Report
- audit credentials for compliance purposes
## Access Analyzer
- identifies whether S3 or IAM role has been shared with *external entity*

# AWS IAM Identity Center
- AWS single Sign-On
- provide centralized access to multiple applications and services for their users
- support SAML 2.0

# AWS KMS (Key Management Service)
- create, manage, control cryptographic keys -> *encryption*
- encrypts EBS

# AWS Secrets Manager
- manage, retrieve, rotate DB credentials, API keys, other screts throughout lifecycles
- automate management and rotation of credentials

# AWS STS (Security Token Service)
- grant temporary, limited-privilege credentials
- no need for long-term access keys or IAM user credentials



++++++++++++++++++
# AWS Support Plan
## Enterprise
- free guidance and support for operational readiness assessment and risk mitigation
- designated technical account manager (TAM) to assist in monitoring and optimization
- email, phone for tech support O
## Business
- email, phone for tech support O
## Developer
- only email for tech support ticket
## Basic
- customer supprt for non-tech issues
- i.e. increase service quotas

# AWS Organizations
- consolidate multiple AWS accounts into an organization
- provides centralized governance and billing for AWS env. including multiple accounts
- create new AWS accounts
- group multiple accounts to organize workflows
- apply policies to groups of accounts

# AWS CloudMap
- creates and maintains a map of backend services

# AWS Systems Manager OpsCenter
- provides central location for IT professionals to view, investigate, and resolve operation work items

# AWS Billing and Cost Management
- AWS Cost and Usage Reports 
  - consolidates the billing in report
  - only work for individual accounts (without cross-account billing)
  - central governance X

# AWS Outposts
- enable to run AWS on on-prem env.
- supports a hybrid architecture
- extend AWS infra, service, APIs and tools to data centers...

# Remote work
- w/ Windows Virtual Desktops and Applications
  - Amazon AppStream 2.0, Amazon WorkSpaces

# Amazon AppStream 2.0
- stream desktop applications securely to a web browser

# AWS Global Accelerator
- improve application availability, performance, security using AWS global network
- helps deliver highly available applications with faast failover for multi-Region and Multi-AZ architectures

++++++++++++++++++
# AWS DMS (Database Migration Service)
- migrate on-prem DB to AWS DB

# AWS AMS (Application Migration Service)
- migrate physical serverws, any DB / Apps to EC2

# AWS Application Discovery Service
- collects info about usage and configuration of on-prem servers to help migrate to AWS

# AWS Migration Hub
- helps plan and track application migrations
- does not perform system migrations

++++++++++++++++++
# Amazon Transcribe
- ML to convert audio 2 text

# Amazon Polly
- ML to convert text 2 speech

# Amazon Translate
- ML to translate language

# Amazon Textract
- ML to extract text from scanend documents

# Amazon Personalize
- ML for personalization

++++++++++++++++++
# AWS Snowmobile
- 50 PTB data transfer from onprem to AWS
