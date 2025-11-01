---
layout: post
title: "🪣 26 AWS security best practices to adopt in production"
---


**AWS IAM**

(1) IAM policies should not allow full “*” administrative privileges

(2) IAM users should not have IAM policies attached

(3) IAM users’ access keys should be rotated every 90 days or less

(4) IAM root user access key should not exist

(5) MFA should be enabled for all IAM users that have a console password

(6) Hardware MFA should be enabled for the root user

(7) Password policies for IAM users should have strong configurations

(8) Unused IAM user credentials should be removed



**Amazon S3**

(9) S3 Block Public Access setting should be enabled

(10) S3 buckets should have server-side encryption enabled

(11) S3 Block Public Access setting should be enabled at the bucket level



**AWS CloudTrail**

(12) CloudTrail should be enabled and configured with at least one multi-Region trail

(13) CloudTrail should have encryption at rest enabled

(14) Ensure CloudTrail log file validation is enabled



**AWS Config**

(15) AWS Config should be enabled



**Amazon EC2**

(16) Attached EBS volumes should be encrypted at rest

(17) VPC flow logging should be enabled in all VPCs

(18) The VPC default security group should not allow inbound and outbound traffic

(19) EBS default encryption should be enabled



**AWS DMS**

(20) AWS Database Migration Service replication instances should not be public



**Amazon EBS**

(21) Amazon EBS snapshots should not be public, determined by the ability to be restorable by anyone



**Amazon OpenSearch Service**

(22) Elasticsearch domains should have encryption at rest enabled



**Amazon SageMaker**

(23) SageMaker notebook instances should not have direct internet access



**AWS Lambda**

(24) Lambda functions should use supported runtimes



**AWS KMS**

(25) AWS KMS keys should not be unintentionally deleted



**Amazon GuardDuty**

(26) GuardDuty should be enabled



---

**🔖 Source** 
- [26 AWS security best practices to adopt in production | Sysdig](https://sysdig.com/blog/26-aws-security-best-practices/)