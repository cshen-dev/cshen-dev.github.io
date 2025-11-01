---
layout: post
title: "24 Google Cloud Platform (GCP) security best practices"
---


1. Check your IAM policies for personal email accounts 🟨
2. Ensure that MFA is enabled for all user accounts 🟥
3. Ensure Security Key enforcement for admin accounts 🟥
4. Prevent the use of user-managed service account keys 🟨
5. Check for anonymously or publicly accessible Cloud KMS keys 🟥
6. Ensure that KMS encryption keys are rotated within a period of 90 days or less 🟩
7. Ensure that Cloud Storage buckets are not anonymously or publicly accessible 🟥
8. Ensure that Cloud Storage buckets have uniform bucket-level access enabled 🟨
9. Enable VPC Flow Logs for VPC Subnets 🟨
10. Ensure “Block Project-wide SSH keys” is enabled for VM instances 🟨
11. Ensure ‘Enable connecting to serial ports’ is not enabled for VM Instance 🟨
12. Ensure VM disks for critical VMs are encrypted with Customer-Supplied Encryption Keys (CSEK) 🟥
13. Enable application-layer secrets encryption for GKE clusters 🟥
14. Enable GKE cluster node encryption with customer-managed keys 🟥
15. Restrict network access to GKE clusters 🟥
16. Ensure that Cloud Audit Logging is configured properly across all services and all users from a project 🟥
17. Ensure that sinks are configured for all log entries 🟨
18. Ensure that retention policies on log buckets are configured using Bucket Lock 🟨
19. Enable logs router encryption with customer-managed keys 🟥
20. Ensure that the Cloud SQL database instance requires all incoming connections to use SSL 🟨
21. Ensure that Cloud SQL database instances are not open to the world 🟥
22. Ensure that Cloud SQL database instances do not have public IPs 🟨
23. Ensure that Cloud SQL database instances are configured with automated backups 🟨
24. Ensure that BigQuery datasets are not anonymously or publicly accessible 🟥

---

**🔖 Source** 
- [24 Google Cloud Platform (GCP) security best practices - Sysdig](https://sysdig.com/learn-cloud-native/24-google-cloud-platform-gcp-security-best-practices/)