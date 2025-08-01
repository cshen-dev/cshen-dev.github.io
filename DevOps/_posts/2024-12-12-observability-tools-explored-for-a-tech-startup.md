---
layout: post
title: "Observability tools explored for a tech startup"
tags: [observability]
---


## Open Source | Self managed Service

| Open Source | Focus | Tech Stack | Comments | 
| ----------- | ----- | ---------- | -------- | 
| Grafana | Visualisation | TypeScript / Golang | Grafana Suite | 
| Loki (Grafana) | Logging | Golang | Grafana Suite |  
| Tempo (Grafana) | Distributed tracing | Golang | Grafana Suite |  
| Prometheus | Metrics | Golang | CNCF |  
| Jeager | Distributed tracing | Golang | CNCF |  
| Elasticsearch | Search (used for logging & metrics) | JVM (Java) | ELK Suite | 
| Logstash | Log collecting | JVM (Java/Ruby) | ELK Suite |  
| Kibana | Visualisation | TypeScript | ELK Suite |  
| Zipkin | Distributed tracing | JVM / TypeScript | from Twitter |  
| Sentry | Error tracking | Python |  |  

## Proprietary | Managed Service

| Proprietary | Focus | Pricing | 
| ----------- | ----- | ------- | 
| Datadog | Strong Infra Monitoring -> Platform | Avg | 
| New Relic | Strong APM -> Platform | Avg |  
| Dynatrace | AI APM -> Platform | Avg |  
| Splunk | Log/Security -> Platform | High |  
| Honeycomb | Distributed tracing | Low |  
| Rollbar | Error tracking | Low |  

## Inbuilt tools from Cloud Computing Providers

| IaaS Inbuilt | Quality | Pricing |
| ------------ | ------- | ------- |
| AWS | hard to use, bad experience | Low |
| GCP | formerly stack driver, better experience | Low |

> To avoid platform lock in and to peruse unified multi cloud dashboard, these inbuilt tools are depreciated. However they will be cheapest out-of-box solution  without too much maintenance effort.

