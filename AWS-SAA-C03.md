


# S3
- cost S3 < EFS < EBS
## Amazon Athena
- allows to run simple SQL questies in S3
- Amazon Athena with workgroups set up
## Amazon AppFlow
- transfer data between SaaS and S3 
## [!Tier!](https://aws.amazon.com/s3/storage-classes-infographic/) (Order by Highest Access Frequency)
### Express One Zone: high performance
- Lowest latency storage for the most frequently accessed data
### Standard: general purpose
- General-purpose storage for active,frequently acceesed data
### Standard-IA: infrequent access
- Low-cost storage for data accessed monthly that requires milliseconds retrieval
### One Zone-IA: infrequent access
- Infrequently accessed data in a single Availability Zone (AZ) for cost savings
- usually as a backup in another Region for disaster recovery
### Glacier Instant Retrieval: archive
- Low-cost storage for long-lived data, with retrieval in milliseconds
### Glacier Flexible Retrieval: archive
- Long-term, low-cost storage for backus, archives, with bulk data retrieval from minutes to hours
### Glacier Deep Archive: archive
- Lowest-cost cloud storage for long-term archived data, with retrieval in hours
### AWS Config
- with appropriate rules, ensure S3 do not have unauthorized configuration changes
## Multipart Upload
- single upload failure -> use multipart upload to S3
## Amazon CloudFront
- reduce data transfer costs by setting it as the origin for S3
### Prevent Direct Access to S3
- set CloudFront as an origin access identity (OAI)
- update the bucket policy to grant permissions to the OAI only
### Transfer Accelerator

# Data
## Amazon Kinesis Data Firehose
- ingest data, uploads data to S3
- persist data on S3
## Amazon Kinesis Data Analytics
- query data(?)
- transforms and analyzes streaming data in real time
- can't use to query specific data
## Amazon Kinesis Data Streams
- capture the data from websites
- handle streaming and clickstream data
- built for high-volume, real-time clickstream analytics
- can't send data to DynamoDB, supports S3, Redshift, OpenSearch Service, Splunk, Datadog...
## AWS Glue
- extract, tranform, and load (ETL) data
- converts the .csv files into Apache Parquet/ORC format


# Storage
## EFS
- Elastic File System
- a simple, durable, scalable, elastic file storage for use with AWS Cloud services and on-prem resources
- can be attached to multiple instances in multiple AZs
### Busting Throughput Mode
- throughput scalses as the size of EFS grows
### Provisioned Throughput Mode
- instantly provision throughput
## EBS
- Elastic Block Store
- an easy-to-use, scalable, high pefrormance block-storage service for Amazon EC2
- can be attached to multiple instances in the same AZ
### EBS Snapshot
- Create and schedule a backup plan with AWS Backup
- Use Amazon Data Lifecycle Manager
### EC2 Modify Volume
- can only expand size
- can change volume type (i.e. io2 to gp3, reduce cost)
  - first use Amazon CloudWatch GetMetricData to get metrics on the underutilized io2 volumes
- does not incur any volume downtime
### Magnetic Volume
- suited for infrequently access
### General Purpose SSD
- up to 16,000 IOPS for each volume
- baseline I/O performance 3 IOPS for each GB
### Provisioned IOPS SSD (io1, io2)
- up to 64,000 IOPS for each volume
- high rate of random disk reads and writes
### Throughput Optimized HDD
- up to 500 IOPS for each volume
### Cold HDD
- defines performance in terms of throughput rather than IOPS
### FSR
- Fast Snapshot Restore
- creates a volume from a snapshot that is fully initialized at creation
- no latency of I/O operations on a first use
## Snowball Edge
- max 80TB, speed up to 100GBps
- 4-6 working days to receive the device
- 2-3 working days to send it back and AWS move the data onto S3
## Snowcone
- max 14TB (SSD configuration)
## Amazon FSx for Lustre File System
- fully managed file system
- designed for high-performance workloads (i.e. gaming apps)

# Container
## Amazon ECS 
- Elastic Container Service
- if uses AWS Fargate for compute, incurs no cost when application idle
- 

# IAM
## PrincipalOrgID
- validates in the principal accessing the resource belongs to an account in your org
## IAM roles, users, groups, AWS STS
- *controls access to AWS resources*
## Amazon Congnito user pools
- *controles access to an application*
- provides authentication, authorization, and user management for web and mobile apps
- users can sign in with a user name and password, or through a trusted third party
## Amazon IAM Identity Center
- two-way trust needed

# Notifications
## Amazon SNS + Amazon SQS
- multiple Amazon SQS queues process messages in parallel

# EC2
## Spot Instance
- Cancel the spot request, THEN Terminate the spot instance
## SSD-Backed Storage Optimized (i2) instance
- higher than 365,000 random IOPS
- instance store has no additional cost
## Auto Scaling
- primary server shouldn't be in a auto scaling group with compute nodes
### With SQS
- set Amazon SQS queue as a destination for jobs
- configure ec2 auto scaling based on the size of the queue
### Default Termination Policy
1. checks which AZ has the most instances
2. identifies at least one instance not protected from scale in
3. (if AZs have equal num of instances) checks for the oldest launch configuration
### Scheduled Scaling Policy
### Suspend-Resume Feature
- if suspend, no more scale out
### Target Tracking Scaling Policy
- creates and manages the Amazon CloudWatch alarms that invoke the scaling policy
- calculates the scaling adjustment based on the metric and the target value

# AWS Global Services
- use AWS global network and its edge locations around te world
- integrates with AWS Shield for DDoS protection
# AWS Global Accelerator
- improves TCP/UDP network performance for cacheable content & dynamic content
- applicable to all around the globe, even if it is deployed in only one region
- content is served at the Global Accelerator edge location
# AWS CloudFront
- improve performance for a wide range of apps over TCP/UDP
- proxying packets at the edge to apps running in one or more AWS regions
- good fit for non-HTTP use cases, such as gaming(UDP), IoT(MQTT), or Voice over IP
- good fit for HTTP use cases, that require static IP addresses
- good fit for HTTP use cases, that require deterministic, fast regional failover

# Elastic Load Balancer
- waits 300 secs before deregistration process
## Application Load Balancer
- can create a listener rule to redirect HTTP traffic to HTTPS
- within a single region
## Network Load Balancer

## Gateway Load Balancer
- designed for deploying "third-party appliances"
- provides a scalable and easy way to route traffic through applicances

# Firewall
## Network Firewall
- creates rules for traffic inspection and traffic filtering

## Firewall Manager
- manages AWS WAF, Shield Advanced, and more

# Network
## VPC
- IPv4-only or dual-stack O, IPv6-only X
- 
## Internet Gateway
- attached to a VPC 
- allow "open internet" traffic into or out of the VPC
- egress-only internet gateway O
## NAT Gateway
- reside within a public subnet, within a single AZ
- allow private EC2 to send requests to the internet
- doesn't support IPv6 traffic
## VPC Peering
- default quota 50, max 125

# VPN
## Site-to-Site VPN
- needs a Customer Gateway and a Virtual Private Gateway
- max 1.25 Gbps
- each connection has 2 tunnels 
### Customer Gateway
- set up and configured in the customer's data center
### Virtual Private Gateway
- attached to VPC to create S2S VPN
### Higher VPN Throughput
- use a transit gateway with equal cost multipath routing, and additional VPN tunnels
## AWS Direct Connect (DX)
### Maximum Resiliency
- configure DX connections at multiple DX locations

# Serverless
## AWS Lambda
- cannot attach EBS volumes
- can mount an EFS file system
## AWS Simple Queue Service (SQS)
- can prioritize polling between 2 queues
### Minimize long-running calls in an external service
- use AWS SQS to offload the long-running requests for asynchronous processing by separate workers
## Amazon Cognito
- provide sign-up and sign-in options for web users and mobile app users


# Database
## Structured for Transactions and Lookups
- Amazon Aurora, Amazon RDS for PostgreSQL
## Structured for Analytics
- Amazon Redshift
  - designed for online analytic processing (OLAP)
## RDS
- multi-AZ set up O
### Provisioned IOPS SSD 
- provides consistent and predictable I/O performance 
### Encryption (ALWAYS, if DB Encryption)
- configure when creating RDS instance
- create snapshot, create encrypted copy of snapshot, restore
## Amazon Neptune
- a graph database service
## Amazon DynamoDB: noSQL DB
- NoSQL - JSON supported
- max item size 400KB
- high read and write rates
- can assign TTL for items 
- supports game platforms with user data, session history...
### Amazon DynamoDB Accelerator (DAX)
- in-memory caching strategy for DynamoDB
- improves read performance for repetitive queries
### On-demand Mode
- can scale to meet sudden increase in demand
### Global Secondary Index
- supports scans and queries at min cost
## Amazon Aurora: RDB
- 5x performance improvment over MySQL on RDS
- auto scaling with Aurora read replicas (for more read requests than write requests)
- multi-AZ O
### Parallel Query
- optimize and speed up query, maintain high throughput for workload
- not cost-effective, always run an instance
### Auto-Scaling
- charges for min of 10 minutes
### Global DB
- create clsters in each additional Region
- RPO of 1 sec, RTOP of less than 1 min
### Serverless
- compute cost per-second basis

# Cache
- cache kb DB data to retuce latency
## Amazon ElasticCache
- provides a fast in-memory data store for use as a DB, cache, message broker, and queue
- supports RDB
### Write-through Strategy
- adds/updates cache data when app writes data to DB
### Lazy-loading Strategy
- loads data into the cache only when necessary
- cache data can get stale

# Migration
## Containerized Apps & PostgreSQL DB
- Migrate the local db to Amazon Aurora Serverless PostgreSQL-Compatible Edition
- Refactor the apps to use Amazon SQS and eliminate the local PostgreSQL dbs
## AWS Database Migration Service (DMS)
- cutover time minimal, AWS DMS keeps the DB in sync
- can be Multi-AZ deployment

# DR
## active/passive:
- Backup and Restore: RPO/RTO Hours
  - backup application, configuration, data to s3
  - when fail, recreate them
- Pilot Light: RPO/RTO 10s of minutes
  - recreates an existing application, stop all ec2
  - start ec2 when fail
- Warm Standby: RPO/RTO Minutes
  - recreates an existing application, keep ec2 alive
  - have live traffic toward the ec2
## active/active: 
- Multi-site active/active: RPO/RTO Real-time

# Security
## Amazon GuardDuty
- threat detection service
- monitors malicious activity and anomalous behavior
## Amazon Inspector
- vulnerability management solution
- identify potential software vulnerabilities
- categorize the severity of vulnerabilities
## AWS Config
### Conformance Packs
- collections of AWS Config rules and remediation actions 
- can deploy as a single entity in an account, a region, across org in AWS Organizations
## AWS Shield Advanced
- expanded DDoS attack protection
- for EC2, ELB, CloudFronts
## Patch
- use AWS Systems Managed Run Command to run a custom command that applies to patch to all EC2 instances

# Monitor
## Amazon CloudWatch
- configure CloudWatch logs to stream data in real-time

# Keys
## AWS Systems Manager Parameter Store
- provides secure, hierarchical storage for configuration data management and secrets management
- secure passwords, DB strings, AMI IDs, licence codes as parameter values
- store as plaintext / encrypted data

# AI
## Amazon Polly
- text 2 speech
- use StartSpeechSynthesisTask API

# Cloud Native Scenarios
## S3 + API Gateway + SQS + Auto Scaling + RDS
- use Amazon S3 to serve the static front-end application
- send requests to Amazon API Gateway, which writes the requests to an Amazon SQS queue
- place the backend instances in an Auto Scaling group
- scale based on the queue length to process and store the data in Amazon RDS
## Kinesis + Lambda + DynamoDB
- high performance, low latency scalable solution
## Test SW Applications
- Apply Amazon Route 53 weighted routing to test the staging environment and gradually increase the traffic as the tests pass.
- Use AWS CloudFormation with a parameter set to the staging value in a separate environment other than the product environment