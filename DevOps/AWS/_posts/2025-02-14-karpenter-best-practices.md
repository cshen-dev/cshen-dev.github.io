---
layout: post
title: "Karpenter Best Practices"
---

## Karpenter Best Practices

1. Use Karpenter for Dynamic Workloads
2. Run Karpenter Controller on EKS Fargate or a Dedicated Node Group
3. Exclude Unnecessary Instance Types
4. Enable Interruption Handling for Spot Instances
5. Configure for Private EKS Clusters
6. Overprovisioning to Improve Responsiveness



## NodePools Best Practices

1. Create Multiple NodePools for Different Requirements
2. Use Mutually Exclusive or Weighted NodePools
3. Use Timers to Automatically Delete Nodes
4. Avoid Overly Constraining Instance Types


## Sources
- [Karpenter: The Ultimate Guide](https://www.perfectscale.io/blog/karpenter)