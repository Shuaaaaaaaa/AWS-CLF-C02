https://www.examtopics.com/exams/amazon/aws-certified-cloud-practitioner-clf-c02/view/2/




++++++++++++++++++
# S3
- data into S3 FREE, Data out of S3 NOT
## Versioning
- preserve, retrieve, restore every version of every objects in S3

# AWS Storage Gateway
- hybrid storage service (connects on-prem with S3)
## AWS File Gateway

# Amazon Macie
- discover and protect sensitive data
- fully managed data security and data privacy service
- uses ML and pattern matching to discover and protect sensitive data

++++++++++++++++++
# Access Keys
- long-term credentials for an IAM user or AWS account root user
- use access keys to sign *programmatic requests to the AWS CLI or AWS API*

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

# AWS CloudTrail
- records all API calls made on your AWS account

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

# AWS Trusted Advisor
- Benefits:
  - Cost optimization, Performance, Security, Fault tolerance, Service quotas

# Amazon Config
- for Compliance

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

# Amazon Aurora
- relational DB

# Amazon DynamoDB
- non-relational DB
- shared responsibility modelx:
  - physical security, patching, encrypting

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
4. Performance Efficiency
5. Cost Optimization

# AWS
- Agility
  - Speed at whch AWS resources are implemented
  - Ability to experiment quickly
- Elasticity
  - Ability to rightsize resources as demand shifts
  - How easily resources can be procured when the are needed

++++++++++++++++++
# AWS Fargate
- serverless compute for containers

++++++++++++++++++
## Internet Gateway
- allow communication between VPC and Internet

# Access
## Assume Role
- EC2 access to S3

# Snowball Edge

# AWS Direct Connect
- dedicated network connection between on-prem and AWS
- no internet inbetween

++++++++++++++++++
# AWS WAF
- deals with common web attack patterns (XSS, SQL Injection, etc...)

# AWS Shiled
- deals with DDoS

# AWS Artifact
- a service to query for security related reports
- provides compliance reports
++++++++++++++++++
# Loosely Coupled Dependencies
- main advantage of moving from *monolithic to microservices*

++++++++++++++++++
# AWS IAM
## Credential Report
- audit credentials for compliance purposes
## Access Analyzer
- identifies whether S3 or IAM role has been shared with external entity

# AWS Organizations
- consolidate multiple AWS accounts into an organization

# AWS STS (Security Token Service)
- grant temporary, limited-privilege credentials
- no need for long-term access keys or IAM user credentials