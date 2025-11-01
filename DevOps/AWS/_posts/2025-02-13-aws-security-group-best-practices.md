---
layout: post
title: "AWS Security Group Best Practices"
---


## Best Practices
- Avoid the use of the “default” security group
- Keep the number of security groups to a minimum
- Restrict, restrict, restrict
- Simplify management
- Develop and enforce a security group monitoring and compliance solution


## Develop a security group strategy

Decide on a clear strategy for creating and using security groups based on your application requirements. Then, use AWS tools to aid enforcement. Examples of options to consider for your strategy are:

- establish the best way to set up your security groups. For example:
  1. one security group per service type, such as “rdp-access”, “ssh-access”, “web”, “active-directory”, “mysql-db”, and then assign the relevant inbound and outbound ports for that service
  2. one security group per application type, such as “web-servers”, “db-servers”, “file-servers”, and then assign the relevant ports for that application
  3. one security group per operating system, such as “windows” or “ubuntu-linux”, and then assign ports common to that OS.

💡 **Pro-tip: you could further sub-divide these into internally and externally facing systems, providing even more flexibility.**

- create one or two default groups that cover access requirements common to all servers in the VPC. Then, enforce the assignment of these to all resources created within that VPC (NB – these should be new groups and not confused with the automatically created AWS “default” group discussed [earlier](https://www.corestack.io/aws-security-best-practices/aws-security-group-best-practices/#_stc6zmeqdplp)). This helps minimise the total number of security groups required. For example:
  1. if all instances need to talk outbound using HTTP / HTTPS to browse the internet
  2. if all instances need to allow an inbound port for a monitoring system. This could be linked to a “monitoring” security group that has outbound access to the custom VPC default group(s)
- the strategy should aim to minimise the number of security groups created and assigned to AWS resources. Otherwise, excessive security group sprawl will make management and troubleshooting difficult
- use a naming strategy that provides clarity and avoids confusion. Remember, it is possible to have multiple peered VPCs. As such, if each VPC has a security group called “web-servers”, it will become difficult to keep track of which one is which


## Sources
- [AWS Security Group: Best Practices & Instructions](https://www.corestack.io/aws-security-best-practices/aws-security-group-best-practices/)