https://www.examtopics.com/exams/amazon/aws-certified-cloud-practitioner-clf-c02/view/2/




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
## Savind Plans
- upfront commitment
- discount up to 72%
## Spot Instances
- for stateless, fault-tolerant workload
- no need to run at speific times

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

++++++++++++++++++
# AWS Glue
- serverless data integration service
- prepare and load data for analysis

# Amazon QuickSight
- business intelligence(BI) at hyperscale
- create and visualize interactive dashboards

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
  - Speed at whch AWS resources are implemented
  - Ability to experiment quickly
- Elasticity
  - Ability to rightsize resources as demand shifts
  - How easily resources can be procured when the are needed

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

++++++++++++++++++
# AWS IAM
## Credential Report
- audit credentials for compliance purposes
## Access Analyzer
- identifies whether S3 or IAM role has been shared with external entity

# AWS KMS (Key Management Service)
- create, manage, control cryptographic keys
- encrypts EBS

# AWS STS (Security Token Service)
- grant temporary, limited-privilege credentials
- no need for long-term access keys or IAM user credentials

# AWS Secrets Manager
- manage, retrieve, rotate DB credentials, API keys, other screts throughout lifecycles

++++++++++++++++++
# AWS Support Plan
## Enterprise
- free guidance and support for operational readiness assessment and risk mitigation
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
