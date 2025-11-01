---
layout: post
title: "📊 Evaluate monitoring tools for an early-stage tech startup in 2024"
tags: [observability]
---

## Introduction

Monitoring is a crucial part of DevOps. As a tech start up grows, we aim to better prepare our organization for enterprise customers who prioritize software reliability and service. Our goal is to eventually establish Service Level Objectives (SLOs) for our applications and infrastructure.

With this objective in mind, I searched the internet and shortlisted 12 tools. I signed up for free trials for most of them and took notes along the way.

Given our small team, with only one dedicated DevOps staff member handling a broad range of requirements, here are some key aspects to focus on when comparing these products:

1. Comprehensive features: We want to integrate as many people as possible onto the platform to reduce silos between Development and Operations.
2. Beginner-friendly: With limited in-house educational resources, the UI should ideally be intuitive and self-explanatory.
3. Low operational effort: With only one DevOps staff member, the tool should require minimal maintenance.
4. Cost-effective: We need to ensure that our observability tools are affordable and within budget.

## Tools evaluated

### [DataDog 💗](https://www.datadoghq.com/)
*for Infrastructure & Application [Estimated monthly price: $1000]*
- Dev Exp: 9/10
- Ops Exp: 8/10
- Cost: 5/10
- Pros
   - Comprehensive product
   - Clear, meaningful graphs
   - Seamless integration of logs and metrics
   - Intuitive navigation UI
   - Offers pipeline insight and LLM
- Cons
   - Expensive, with reports of hidden charges

### [NewRelic 💛](https://newrelic.com/)
*for Infrastructure & Application [Estimated monthly price: $500]*
- Dev Exp: 8/10
- Ops Exp: 8/10
- Cost: 7/10
- Pros
   - Intuitive UI and graphs
   - Feature-rich, including mobile and digital experience sectors
   - More reasonable pricing compared to DataDog
- Cons
   - Charges per seat and data ingestion
   - Historically an APM company, not sure if conservative
   - Customer service quality is uncertain

### [SigNoz 💚  (opensource)](https://signoz.io/)
*for Infrastructure & Application  [Estimated monthly price: $200]*
- Dev Exp: 7/10
- Ops Exp: 9/10
- Cost: 9/10
- Pros
   - Open-source and can be self-hosted
   - All-in-one solution, unlike Grafana/Elastic which require multiple components
   - Uses ClickHouse as backend, cost-efficient and future-proof
- Cons
   - Managed service is relatively new compared to bigger players
   - Lacks digital experience monitoring

### [Grafana Stack 💚 (opensource)](https://grafana.com/)
*Infrastructure-focused & Application covered  [Estimated monthly price: $0]*
- Dev Exp: 6/10
- Ops Exp: 7/10
- Cost: 10/10
- Pros
   - Cloud-native
   - Integrates well with Prometheus, focusing on Kubernetes
   - Very cost-effective due to its popularity
- Cons
   - UI is laggy and complex compared to SigNoz
   - Poor log management, especially for log searching

### [Elastic Stack 💙  (opensource)](https://www.elastic.co/)
*Log-focused & Metrics covered [Estimated monthly price: $800]*
- Dev Exp: 6/10
- Ops Exp: 5/10
- Cost: 6/10
- Pros
   - Popular log management tool
   - Offers SEIM for security
   - Includes APM, which has improved over the years
   - Affordable among big names
- Cons
   - Generic tools focusing on log analytics
   - Requires extra effort to configure as an observability tool
   - Resource-heavy, especially its database

### [Sentry ⏹️](https://sentry.io/welcome/)  
*Application performance-focused*
- Pause as it is a speclised tool as opposed to a suite
- Pros
   - Leading error capturing product
- Cons
   - Does not cover infrastructure

### [Honeycomb ⏹️](https://www.honeycomb.io/)
*Application performance-focused*
- Pause as it is a speclised tool as opposed to a suite
- Pros
   - Leading observability company
   - Great product vision
   - Cost-effective
- Cons
   - Does not cover infrastructure & dashboard well

### [Better Stack ⏹️](https://betterstack.com/)
*Uptime monitoing & Logs & Metric*
- Pause as it is a speclised tool as opposed to a suite
- Pros
   - Matches our current needs perfectly
   - Sleek UI
- Cons
   - Kubernetes integration requires additional support
   - Less technical appearance compared to other options

### [Dynatrace ❌](https://www.dynatrace.com/) 
*for Infrastructure & Application*
- Drop for the Enterprise Price Plan
- Microsoft-like UI, feels like an extension of Windows
- Enterprise-level complexity
- Potentially high enterprise-level cost

### [Logz.io ❌](https://logz.io/)  
*for Infrastructure & Application*
- Drop for the technical complexity
- Combines the complexity of the ELK and Grafana stacks
- Resource-heavy due to bundling multiple open-source projects

### [Splunk ❌](https://www.splunk.com/) 
*Secure-focused Log analytic platform*
- Drop for the Enterprise Price Plan
- Leading company in SEIM with high adoption in the security industry
- High enterprise-level cost
- Cisco product


## Legends

💗 Attractive

💛 Like

💚 Safe choice

💙 Mixed feelings (I feel blue when using them)

⏹️ Limited for certain aspects

❌ Not recommended

## Conclusion

Datadog is a well-rounded product that can effectively bridge the gap between development and operations. However, its notoriously high costs are a significant concern.

NewRelic offers a middle ground between proprietary and open-source products. It is much more affordable than Datadog while providing similar features, and we can still benefit from their engineering support.

Signoz is the ideal choice if we want to adopt an open-source product and potentially self-host it in the future. Its use of ClickHouse for data storage aligns well with our operational goals.

