# aws-certified-developer-exam-tips
A list of knowledge areas per AWS service that should be remembered for the AWS Certified Developer - Associate exam

# IAM
* Never use the IAM root account for day-to-day activities
* Always setup MFA on the IAM root account
* Use IAM Policy Simulator to test out permission levels
* Know the usage scope of IAM Managed Policies, Customer Managed Policies and Inline Policies

# EC2
* Have an understanding of which EC2 pricing options to use and when
* Have an understanding of the different EBS volume types and when to use cases
* Know the differences between the ELB types
* Know that you need `x-forwarded-for` for IP tracking and Sticky Sessions for session management
* Never store IAM programmatic keys on an EC2 instances or within code

# RDS
* Understand the difference between read-replicas and multi-AZ for RDS
* Know the difference between Automated Backups and Snapshots in RDS

# ElasticCache
* Know the 2 types of ElastiCache offerings and when to use ElastiCache

# Secrets
* Know the difference between Secrets Manager Parameter Store and Secrets Manager

# S3
* Understand the S3 storage classes and tradeoffs
* Understand S3 encryption options and how these are implemented
* Be confident about how to use the `x-amz-server-side-encryption` parameter with bucket policies and request headers
* Understand why CORS is important in S3

# CloudFront
* Be familiar with CloudFront Origin, Distribution, Edge Location, and TTL

# Lambda
* Understand Lambda versioning, using Lambda in a VPC, and concurrent execution limits
* Know the errors returned when Lambda concurrency executions are exhausted

# API Gateway
* Be knowledgeable about API Gateway and the API Types it supports, Caching, and Throttling
* Know the errors returned when API Gateway is thorttled

# X-Ray
* Be familiar with X-Ray and how it is configured for Lambda, EC2 and Containers (and where)

# DynamoDB
* Know your DynamoDB calculations for RCU and WCU well - practice this repeatedly, it will come up on the exam
* Know that Eventually Consistent reads are better for **read performance** and Strongly Consistent reads are better for **read consistency**
* Be comfortable choosing a partition key
* Be comfortable choosing a composite key
* Know when to use Scan vs Query
* Know difference between Local Secondary Index and Global Secondary Index
* Know when to use DynamoDB Accelerator and where to place this in an architecture
* Know about DynamoDB streams and its use case
* Be familar with the errors returned when provisioned throughput has exceeded

# KMS
* Understand envelope encryption with KMS
* Understand CMK usage patterns with KMS

# SQS / SNS / SQS
* Know the difference between long polling and short polling with SQS
* Know that SQS is pull based and SNS is push based
* Know the message size limits, maximum days of retention and default days of retention in SQS
* Know the difference queue types in SQS and what makes them different
* Understand visibility timeout, the default value, the maxmium value and how it is used in a scenario
* Understand SQS delay queues
* Know that SES is a service and when it can be used

# Kinesis
* Know the difference between Kinesis Data Streams, Data Analytics and Data Streams
* Understand how Shards and Consumers are configured, particularly about the number of record processors

# Elastic Beanstalk
* Understand Elastic Beanstalk and its use case
* Understand the Elastic Beanstalk deployment options well, along with selecting the best option for a given scenario
* Know that you can have RDS inside or outside of an Elastic Beanstalk and its tradeoffs

# CI/CD
* Understand when to use CodeCommit, CodeBuild, CodeDeploy and CodePipeline
* Know the deployment options of CodePipeline
* Understand the CodeDeploy Lifecycle Event Hooks well

# ECS / ECR
* Understand ECS and its advantages offered
* Know the basics of ECR and how to build, tag and push docker images to ECR
* Know how to deploy Docker using Elastic Beanstalk

# CloudFormation
* Be comfortable with CloudFormation, the template structure and Nested Stacks
* Understand how CloudFormation and SAM work together

# Cognito
* Understand how to apply User Pools and Identity Pools to scenarios using Cognito

# CloudWatch
* Understand the basics of CloudWatch, the default metrics and intervals, Custom Metrics and options available
* Know the difference between CloudWatch and CloudTrail
