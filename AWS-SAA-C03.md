


# S3
## Amazon Athena
- integrates seamlessly with S3
- allows to run simple SQL questies in no time


# Storage
## EFS
- Elastic File System
- a simple, scalable, elastic file storage for use with AWS Cloud services and on-prem resources
## EBS
- Elastic Block Store
- an easy-to-use, scalable, high pefrormance block-storage service for Amazon EC2
### General Purpose SSD
- up to 16,000 IOPS for each volume
- baseline I/O performance 3 IOPS for each GB
### Provisioned IOPS SSD
- up to 64,000 IOPS for each volume
### Throughput Optimized HDD
- up to 500 IOPS for each volume
### Cold HDD
- defines performance in terms of throughput rather than IOPS
### FSR
- Fast Snapshot Restore
- creates a volume from a snapshot that is fully initialized at creation
- no latency of I/O operations on a first use
## Snowball Edge
- speed up to 100GBps
- 4-6 working days to receive the device
- 2-3 working days to send it back and AWS move the data onto S3

# DB
## Amazon Aurora
- 5x performance improvment over MySQL on RDS
- auto scaling with Aurora read replicas (for more read requests than write requests)
### Serverless
- no compute cost when idle

# Container
## Amazon ECS 
- Elastic Container Service
- if uses AWS Fargate for compute, incurs no cost when application idle

# IAM
## PrincipalOrgID
- validates in the principal accessing the resource belongs to an account in your org
## IAM roles, users, groups, AWS STS
- *controls access to AWS resources*
## Amazon Congnito user pools
- *controles access to an application*
- provides authentication, authorization, and user management for web and mobile apps
- users can sign in with a user name and password, or through a trusted third party

# Notifications
## Amazon SNS + Amazon SQS
- multiple Amazon SQS queues process messages in parallel

# EC2
## Auto Scaling
- primary server shouldn't be in a auto scaling group with compute nodes
- scenario with Amazon SQS:
  - set Amazon SQS queue as a destination for jobs
  - configure ec2 auto scaling based on the size of the queue

# AWS Global Services
- use AWS global network and its edge locations around te world
- integrates with AWS Shield for DDoS protection
# AWS Global Accelerator
- improves performance for cacheable content & dynamic content
- content is served at the edge
# AWS CloudFront
- improve performance for a wide range of apps over TCP/UDP
- proxying packets at the edge to apps running in one or more AWS regions
- good fit for non-HTTP use cases, such as gaming(UDP), IoT(MQTT), or Voice over IP
- good fit for HTTP use cases, that require static IP addresses
- good fit for HTTP use cases, that require deterministic, fast regional failover

# LB
## Application Load Balancer

## Network Load Balancer

## Gateway Load Balancer
- designed for deploying third-party appliances
- provides a scalable and easy way to route traffic through applicances

# Firewall
## Network Firewall
- creates rules for traffic inspection and traffic filtering

## Firewall Manager
- manages AWS WAF, Shield Advanced, and more

# Network
## Internet Gateway
- attached to a VPC 
- allow "open internet" traffic into or out of the VPC
## NAT Gateway
- allow private EC2 to send requests to the internet
 

# VPN
## Site-to-Site VPN
- needs a Customer Gateway and a Virtual Private Gateway
### Customer Gateway
- set up and configured in the customer's data center
### Virtual Private Gateway
- attached to VPC to create S2S VPN
- 





+++++++++++++++++++++++++=
AWS Certified Solutions Architect - Associate Official Practice Question Set (SAA-C03)

# DR
## Warm Standby
- RTO of 5 mins
- instances run at a low capacity and can scale within minutes
## Pilot Light
- RTO can't be 5 mins
## Multi-site active-active
- RTO within moments
- costs more
## Backup and Restore
- RTO can't be 5 mins

# Security
## Amazon GuardDuty
- threat detection service
- monitors malicious activity and anomalous behavior
## Amazon Inspector
- vulnerability management solution
- identify potential software vulnerabilities
- categorize the severity of vulnerabilities
- 