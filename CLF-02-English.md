Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 Time Elapsed: 00:09
Done Reviewing
 
1/20
 
Question
A company wants to establish a consistent and private connection from the company's on-premises data center to the AWS Cloud.

Which AWS service will meet these requirements?

Report Content Errors

A
AWS Client VPN

Incorrect. Client VPN is a managed client-based VPN service that gives you the ability to securely access your AWS resources and the resources in your on-premises network. With Client VPN, you can access your resources from any location through an OpenVPN-based VPN client. You would use Client VPN to connect individual laptops to AWS, not an entire data center.

Learn more about Client VPN.


B
Amazon Connect

Incorrect. Amazon Connect is an omnichannel cloud contact center that helps you provide superior customer service at a lower cost. Amazon Connect provides a seamless experience across voice and chat for your customers and agents. Amazon Connect is not a service that connects an on-premises network to AWS.

Learn more about Amazon Connect.


C
AWS Direct Connect

Correct. Direct Connect links your internal network to a Direct Connect location through a standard Ethernet fiber-optic cable. One end of the cable connects to your router. The other end of the cable connects to a Direct Connect router. AWS Direct Connect is consistent and private because your company is the only user of the cable.

Learn more about Direct Connect.


D
AWS Site-to-Site VPN

Incorrect. Site-to-Site VPN creates an encrypted network path between your on-premises network and your AWS Cloud network. This connection uses the internet, so you cannot expect consistency. Even though the traffic is encrypted, the connection is not private because the internet is a shared resource.

Learn more about Site-to-Site VPN.

Correct
Your Answer:
C
Correct Answer:
C
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

++++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:27
 Total: 00:36
Pause Exam
2/20
5.0% complete

Question
A user needs to automatically discover, classify, and protect sensitive data stored in Amazon S3.

Which AWS service can meet these requirements?

Report Content Errors

A
Amazon Inspector

Incorrect. Amazon Inspector is an automated security assessment service that helps improve the security and compliance of applications deployed on Amazon EC2 instances. Amazon Inspector does not perform S3 data classification and automatic discovery.

Learn more about Amazon Inspector.


B
Amazon Macie

Correct. Macie is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS.

Learn more about Macie.


C
Amazon GuardDuty

Incorrect. GuardDuty is a threat detection service that continuously monitors for malicious activity and unauthorized behavior to protect your AWS accounts and workloads. GuardDuty does not perform S3 data classification.

Learn more about GuardDuty.


D
AWS Secrets Manager

Incorrect. Secrets Manager helps you protect secrets needed to access your applications, services, and IT resources. Secrets Manager does not perform S3 data classification and automatic discovery.

Learn more about Secrets Manager.

Correct
Your Answer:
B
Correct Answer:
B
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

++++++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:26
 Total: 01:02
Pause Exam
3/20
10.0% complete

Question
A company has an on-premises Linux-based server with an Oracle database that runs on it. The company wants to migrate the database server to run on an Amazon EC2 instance in AWS.

Which service should the company use to complete the migration?

Report Content Errors

A
AWS Database Migration Service (AWS DMS)

Incorrect. AWS DMS can be used to migrate data from an on-premises database to a database in AWS. However, AWS DMS does not migrate the actual server to an EC2 instance.

Learn more about AWS DMS.


B
AWS Migration Hub

Incorrect. Migration Hub is a service that helps plan and track application migrations. Migration Hub does not perform system migrations.

Learn more about Migration Hub.


C
AWS Application Migration Service (AWS MGN)

Correct. AWS MGN is an automated lift-and-shift solution. This solution can migrate physical servers and any databases or applications that run on them to EC2 instances in AWS.

Learn more about AWS MGN.


D
AWS Application Discovery Service

Incorrect. Application Discovery Service collects information about the usage and configuration of on-premises servers to help plan a migration to AWS. Application Discovery Service does not actually perform migration operations.

Learn more about Application Discovery Service.

Incorrect
Your Answer:
A
Correct Answer:
C
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

+++++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:14
 Total: 01:17
Pause Exam
4/20
15.0% complete

Question
A company wants to create a learning application for students. The learning application must give students the option to choose a button to have the text read out loud to them.

Which AWS machine learning service will meet this requirement?

Report Content Errors

A
Amazon Transcribe

Incorrect. Amazon Transcribe is a service that uses machine learning to convert audio data to text. Amazon Transcribe is not a text-to-speech conversion service.

Learn more about Amazon Transcribe.


B
Amazon Polly

Correct. Amazon Polly is a machine learning service that converts text to speech. This service provides the ability to read text out loud.

Learn more about Amazon Polly.


C
Amazon Translate

Incorrect. Amazon Translate is a machine learning language translation service. Amazon Translate is not a text-to-speech conversion service.

Learn more about Amazon Translate.


D
Amazon Textract

Incorrect. Amazon Textract is a machine learning service that can extract text from scanned documents. Amazon Textract is not a text-to-speech conversion service.

Learn more about Amazon Textract.

Incorrect
Your Answer:
A
Correct Answer:
B
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

+++++++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:16
 Total: 01:33
Pause Exam
5/20
20.0% complete

Question
What are the advantages of deploying an application with Amazon EC2 instances in multiple Availability Zones? (Select TWO.)

Report Content Errors

A
Preventing a single point of failure

Correct. The deployment of the EC2 instances in multiple Availability Zones prevents a single point of failure. Availability Zones are designed for physical redundancy and to provide resilience with uninterrupted performance.

Learn more about Availability Zones.


B
Reducing the operational costs of the application

Incorrect. Multiple Availability Zones prevent single points of failure. As a result, the overall availability of the application improves. Multiple Availability Zones will not reduce the operational costs of the application.


C
Allowing the application to serve cross-Region users with low latency

Incorrect. The best option to serve users with low latency across Regions is to launch another EC2 instance in the second Region that is closer to the user's location.


D
Increasing the availability of the application

Correct. If you host all your instances in a single location that is affected by a failure, none of your instances would be available. Availability Zones are designed for physical redundancy and to provide resilience with uninterrupted performance.

Learn more about Availability Zones.


E
Increasing the load of the application

Incorrect. Multiple Availability Zones will prevent single points of failure. As a result, the overall availability of the application will improve. However, two EC2 instances that run in the same Availability Zone or in different Availability Zones will not change the overall load of the application.

Correct
Your Answer:
AD
Correct Answer:
AD
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:21
 Total: 01:54
Pause Exam
6/20
25.0% complete

Question
How does AWS charge for AWS Lambda usage once the free tier has been exceeded? (Select TWO.)

Report Content Errors

A
By the time it takes for the Lambda function to run

Correct. Lambda charges are dependent on the amount of time it takes to run the code.

Learn more about Lambda pricing.

Learn more about Lambda.


B
By the number of versions of a specific Lambda function

Incorrect. The number of versions of a specific Lambda function does not contribute to the cost. You are charged based on the number of requests for your Lambda functions and the duration of time it takes for your code to run.


C
By the number of requests made for a given Lambda function

Correct. Lambda charges are dependent on the number of requests for your Lambda functions.

Learn more about Lambda pricing.

Learn more about Lambda.


D
By the programming language that is used for the Lambda function

Incorrect. The programming language that is used to create the Lambda function does not contribute to the cost. You are charged based on the number of requests for your Lambda functions and the duration of time it takes for your code to run.


E
By the total number of Lambda functions in an AWS account

Incorrect. There is no charge based on the number of functions in an AWS account. You are charged based on the number of requests for your Lambda functions and the duration of time it takes for your code to run.

Correct
Your Answer:
AC
Correct Answer:
AC
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

++++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 01:19
 Total: 03:14
Pause Exam
7/20
30.0% complete

Question
A company requires a relational database on AWS that records new customer orders from a website.

Which AWS service or feature will meet this requirement?

Report Content Errors

A
AWS Global Accelerator

Incorrect. Global Accelerator is a networking service that improves the performance of your users’ network traffic by up to 60%. Global Accelerator uses the AWS global network infrastructure. Global Accelerator is not a relational database.

Learn more about Global Accelerator.


B
Amazon DynamoDB

Incorrect. DynamoDB is a fully managed NoSQL database service. DynamoDB provides fast and predictable performance with seamless scalability. However, DynamoDB is not a relational database.

Learn more about DynamoDB.


C
Amazon Aurora

Correct. Aurora is a MySQL- and PostgreSQL-compatible relational database built for the cloud. Aurora combines the performance and availability of traditional enterprise databases with the simplicity and cost-effectiveness of open source databases.

Learn more about Aurora.


D
Amazon Elastic Block Store (Amazon EBS)

Incorrect. Amazon EBS is an easy-to-use, high-performance block-storage service. You can use Amazon EBS with Amazon EC2 for both throughput- and transaction-intensive workloads at any scale. You can run a database on Amazon EC2 instances and use Amazon EBS for the storage for that database. However, Amazon EBS by itself is not a relational database.

Learn more about Amazon EBS.

Correct
Your Answer:
C
Correct Answer:
C
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

++++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:23
 Total: 03:38
Pause Exam
8/20
35.0% complete

Question
A user deploys an Amazon RDS DB instance in multiple Availability Zones.

This strategy involves which pillar of the AWS Well-Architected Framework?

Report Content Errors

A
Performance efficiency

Incorrect. The performance efficiency pillar includes the ability to use computing resources efficiently to meet system requirements, and to maintain that efficiency as demand changes and technologies evolve. The use of multiple Availability Zones does not increase performance efficiency.

Learn more about performance efficiency.


B
Reliability

Correct. The reliability pillar includes the ability of a workload to perform its intended function correctly and consistently when it is expected to do so. The deployment of Amazon RDS in multiple Availability Zones supports the goal of reliability because it reduces single points of failure.

Learn more about reliability.


C
Cost optimization

Incorrect. The cost optimization pillar includes the ability to run systems to deliver business value at the lowest price point. Reliability is supported by using resources in multiple Availability Zones. The use of multiple Availability Zones for resources will increase cost.

Learn more about cost optimization.


D
Security

Incorrect. The security pillar includes the ability to protect data, systems, and assets to take advantage of cloud technologies to improve a company's security. The use of multiple Availability Zones for resources does not make an application more secure.

Learn more about security.

Incorrect
Your Answer:
A
Correct Answer:
B
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

+++++++++++++=
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:34
 Total: 04:12
Pause Exam
9/20
40.0% complete

Question
A company needs to monitor and receive alerts about AWS Management Console sign-in events that involve the AWS account root user.

Which AWS service can the company use to meet these requirements?

Report Content Errors

A
Amazon CloudWatch

Correct. CloudWatch monitors your AWS resources and the applications that you run on AWS in real time. You can use CloudWatch with AWS CloudTrail to monitor and receive alerts about console sign-in events that involve the AWS account root user.

Learn more about CloudWatch.

Learn more about CloudTrail.


B
AWS Config

Incorrect. You can use AWS Config to assess, audit, and evaluate the configurations of your AWS resources. AWS Config cannot alert you about console sign-in events that involve the AWS account root user.

Learn more about AWS Config.


C
AWS Trusted Advisor

Incorrect. You can use Trusted Advisor for real-time guidance to help you provision your resources according to AWS best practices. Trusted Advisor cannot alert you about console sign-in events that involve the AWS account root user.

Learn more about Trusted Advisor.


D
AWS Identity and Access Management (IAM)

Incorrect. With IAM, you can manage access to AWS services and resources securely. IAM cannot alert you about console sign-in events that involve the AWS account root user.

Learn more about IAM.

Incorrect
Your Answer:
D
Correct Answer:
A
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

+++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:14
 Total: 04:26
Pause Exam
10/20
45.0% complete

Question
Which credential components are required to gain programmatic access to an AWS account? (Select TWO.)

Report Content Errors

A
An access key ID

Correct. Programmatic access requires an access key ID and a secret access key that can be assigned to an AWS user.

Learn more about access key best practices.


B
A primary key

Incorrect. A primary key is a feature used in database management. It does not grant AWS account access.

Learn more about AWS security credentials.


C
A secret access key

Correct. Programmatic access requires an access key ID and a secret access key that can be assigned to an AWS user.

Learn more about access key best practices.


D
A user ID

Incorrect. A user ID is used for IAM security credentials, but not for programmatic access.

Learn more about IAM users.


E
A secondary key

Incorrect. A secondary key is a feature used in database management. It does not grant AWS account access.

Learn more about AWS security credentials.

Correct
Your Answer:
AC
Correct Answer:
AC
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:14
 Total: 04:41
Pause Exam
11/20
50.0% complete

Question
What is the MINIMUM AWS Support plan that provides technical support through phone calls?

Report Content Errors

A
Enterprise

Incorrect. The Enterprise Support plan provides phone support, but it is not the minimum plan to do so.


B
Business

Correct. You can call or chat with technical support by using the Business Support plan or the Enterprise Support plan. The Business Support plan is the minimum plan that provides this feature.

Learn more about AWS Support plans. 


C
Developer

Incorrect. The Developer Support plan allows only email creation of support tickets and does not provide phone support.


D
Basic

Incorrect. The Basic Support plan provides customer support for non-technical issues, such as increases in service quotas. However, the Basic Support plan does not provide technical support.

Correct
Your Answer:
B
Correct Answer:
B
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

++++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:47
 Total: 05:28
Pause Exam
12/20
55.0% complete

Question
A company is hosting a static website from a single Amazon S3 bucket. 

Which AWS service will achieve lower latency and high transfer speeds?

Report Content Errors

A
AWS Elastic Beanstalk

Incorrect. Elastic Beanstalk is a service to deploy and scale web applications and services developed with common programming languages on automatically deployed infrastructure with capacity management, load balancing, auto scaling, and monitoring. Elastic Beanstalk makes it easier to provision and support an application. Elastic Beanstalk does not reduce website latency.

Learn more about Elastic Beanstalk.


B
Amazon DynamoDB Accelerator (DAX)

Incorrect. DAX is used to reduce response times from a DynamoDB table from single-digit milliseconds to microseconds. DynamoDB tables cannot host static websites.

Learn more about DAX.


C
Amazon Route 53

Incorrect. Route 53 is a highly available and scalable DNS web service. The three main functions of Route 53 are registering domain names, routing internet traffic to the resources for your domain, and checking the health of those resources. Route 53 can direct traffic to S3 buckets. But because the question describes only one S3 bucket, Route 53 would have only one potential route and could not reduce latency.

Learn more about Route 53.

Learn more about how to route to S3 buckets with Route 53.


D
Amazon CloudFront

Correct. CloudFront is a web service that speeds up the distribution of your static and dynamic web content, such as .html, .css, .js, and image files, to your users. Content is cached in edge locations. Content that is repeatedly accessed can be served from the edge locations instead of the source S3 bucket.

Learn more about CloudFront.

Correct
Your Answer:
D
Correct Answer:
D
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

+++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:24
 Total: 05:52
Pause Exam
13/20
60.0% complete

Question
Which AWS service identifies security groups that allow unrestricted access to a user's AWS resources?

Report Content Errors

A
AWS Trusted Advisor

Correct. Trusted Advisor checks security groups for rules that allow unrestricted access to a resource. Unrestricted access increases opportunities for malicious activity, such as hacking, denial-of-service attacks, or loss of data. 

Learn more about Trusted Advisor checks.


B
AWS Config
Incorrect. AWS Config continuously monitors and records changes to your AWS resources, but it does not identify security groups that allow unrestricted access.

Learn more about AWS Config.


C
Amazon CloudWatch

Incorrect. CloudWatch is a monitoring service that collects and tracks metrics for AWS resources. It does not identify security groups that allow unrestricted access.

Learn more about CloudWatch.


D
AWS CloudTrail

Incorrect. CloudTrail provides an audit record of API calls. It does not identify security groups that allow unrestricted access.

Learn more about CloudTrail.

Correct
Your Answer:
A
Correct Answer:
A
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

+++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 03:17
 Total: 09:10
Pause Exam
14/20
65.0% complete

Question
Which of the functionalities are characteristics of Amazon S3? (Select TWO.)

Report Content Errors

A
A global file system

Incorrect. Amazon S3 is not a global file system. Amazon S3 is an object storage service.

Learn more about Amazon S3.


B
An object store

Correct. Amazon S3 is an object storage service.

Learn more about Amazon S3.


C
A local file store

Incorrect. Amazon S3 is not a local file store. Amazon S3 is an object storage service.

Learn more about Amazon S3.


D
A network file system

Incorrect. Amazon S3 is not a network file system. Amazon S3 is an object storage service.

Learn more about Amazon S3.


E
A durable storage system

Correct. Amazon S3 is a durable object storage service.

Learn more about data protection in Amazon S3.

Correct
Your Answer:
BE
Correct Answer:
BE
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

++++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:23
 Total: 09:39
Pause Exam
16/20
75.0% complete

Question
Which AWS service allows customers to purchase unused Amazon EC2 capacity at an often discounted rate?

Report Content Errors

A
Reserved Instances

Incorrect. Reserved Instances reserve some capacity for your use at any time. Reserved Instances can sometimes give you a discount. However, this capacity is not unused capacity.

Learn more about Reserved Instances.


B
On-Demand Instances

Incorrect. On-Demand Instances are the default purchase option and are immediately available. On-Demand Instances are not discounted.

Learn more about On-Demand Instances.


C
Dedicated Instances

Incorrect. Dedicated Instances run in VPCs on hardware dedicated to that individual customer and are often used when there are licensing or compliance constraints. Dedicated Instances are not discounted.

Learn more about Dedicated Instances.


D
Spot Instances

Correct. With Spot Instances, you can access unused EC2 capacity. Spot Instances can be discounted.

Learn more about Spot Instances.

Correct
Your Answer:
D
Correct Answer:
D
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

++++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:10
 Total: 09:50
Pause Exam
17/20
80.0% complete

Question
Which tasks are the customer's responsibility according to the AWS shared responsibility model? (Select TWO.)

Report Content Errors

A
Patch the operating system that AWS Lambda functions use.

Incorrect. AWS provides Lambda as a service. The customer does not have to patch the operating system.

Learn more about the Shared Responsibility Model.


B
Install patches on Amazon RDS DB instances.

Incorrect. AWS provides Amazon RDS as a service. AWS manages patches for the Amazon RDS engine. The customer can choose a time window to install patches.

Learn more about patch management for Amazon RDS.


C
Control physical access to the data center that contains a customer's VPC.

Incorrect. AWS does not allow access to data centers. A customer can take a virtual tour of a data center to understand the security measures and controls. Customers cannot visit data centers in person.

Learn more about AWS data centers.


D
Configure IAM users according to the principle of least privilege.

Correct. AWS provides AWS Identity and Access Management (IAM) as a service. The customer defines IAM users and the access policies that apply to those users.

Learn more about the Shared Responsibility Model.


E
Configure an Amazon S3 bucket to allow public access.

Correct. The customer determines access permissions to S3 buckets that the customer owns.  

Learn more about the Shared Responsibility Model.

Correct
Your Answer:
DE
Correct Answer:
DE
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:20
 Total: 10:10
Pause Exam
18/20
85.0% complete

Question
A company is moving all of their development activities to AWS. The company wants a solution to store and manage their developers' source code.

Which AWS coding service will meet this requirement?

Report Content Errors

A
AWS CodeArtifact

Incorrect. CodeArtifact is a managed artifact repository service that stores and shares software that is ready for deployment. CodeArtifact is not a source code management service.

Learn more about CodeArtifact.


B
AWS CodeBuild

Incorrect. CodeBuild is a service that helps users to automatically compile source code, run unit tests, and produce software packages that are ready for deployment. CodeBuild is not a code management service.

Learn more about CodeBuild.


C
AWS CodePipeline

Incorrect. CodePipeline is a service that manages the movement of code between the individual services. CodePipeline is not a source code storage service.

Learn more about CodePipeline.


D
AWS CodeCommit

Correct. CodeCommit is a source code version control service. CodeCommit helps users store and manage developers' source code in AWS.

Learn more about CodeCommit.

Incorrect
Your Answer:
A
Correct Answer:
D
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

+++++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:39
 Total: 10:50
Pause Exam
19/20
90.0% complete

Question
What are benefits of using the AWS Cloud for companies with customers in many countries around the world? (Select TWO.)

Report Content Errors

A
Companies can deploy applications in multiple AWS Regions to reduce latency.

Correct. The use of Regions around the world will improve an application's global performance and reduce latency for users.

Learn more about AWS Global Infrastructure.

Learn more about AWS Regions.


B
Amazon Translate automatically translates third-party website interfaces into multiple languages.

Incorrect. Amazon Translate does not provide automatic translation of third-party website interfaces.

Learn more about Amazon Translate.


C
Amazon CloudFront has multiple edge locations around the world to reduce latency.

Correct. CloudFront is a content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to global customers with low latency and high transfer speeds.

Learn more about how CloudFront delivers content.

Learn more about the CloudFront edge network.


D
Amazon Comprehend allows users to build applications that can respond to user requests in many languages.

Incorrect. Amazon Comprehend is a natural language processing (NLP) service that uses machine learning to find insights and relationships in text. Amazon Comprehend does not translate text.

Learn more about Amazon Comprehend.


E
Elastic Load Balancing can distribute application web traffic to multiple AWS Regions around the world, which reduces latency.

Incorrect. A load balancer accepts incoming traffic from clients and routes requests to its registered targets (such as EC2 instances) in one or more Availability Zones. However, a load balancer does not accept targets across Regions.

Learn more about Elastic Load Balancing.

Correct
Your Answer:
AC
Correct Answer:
AC
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.

++++++++++++
Skip to main content

 
AWS Certified Cloud Practitioner Official Practice Question Set (CLF-C02-English)
 This Question: 00:14
 Total: 11:05
Pause Exam
20/20
95.0% complete

Question
Each department within a company has its own independent AWS account and its own payment method. The company needs to centralize departmental governance and consolidate payments.

How can the company achieve these objectives by using AWS services or features?

Report Content Errors

A
Use AWS Cloud Map on each departmental account.

Incorrect. AWS Cloud Map creates and maintains a map of backend services. AWS Cloud Map will not address governance or payment consolidation.

Learn more about AWS Cloud Map.


B
Create an organization in AWS Organizations with all features enabled within one account. Invite all accounts to join the organization.

Correct. Organizations provides centralized governance and billing for an AWS environment, including multiple accounts.

Learn more about Organizations.


C
Use AWS Systems Manager OpsCenter.

Incorrect. OpsCenter provides a central location for IT professionals to view, investigate, and resolve operational work items. OpsCenter does not consolidate billing.

Learn more about OpsCenter.


D
Use the AWS Cost and Usage Reports page of the AWS Billing and Cost Management console.

Incorrect. This solution consolidates the billing in a report, but it will work only for the individual accounts (without cross-account billing). This solution does not address central governance.

Learn more about Cost and Usage Reports.

Incorrect
Your Answer:
D
Correct Answer:
B
Continue
 Close
Legal Privacy Support
©2022, Amazon Web Services, Inc. or its affiliates. All rights reserved.