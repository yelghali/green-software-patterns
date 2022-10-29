---
version: 1.0
submitted_by: yelghali
published_date: tbd
category: cloud
tags: 
- serverless
- kubernetes
- role:software-engineer
- role:cloud-engineer
- size:medium
---

# Scale Kubernetes workloads based on events

## Description
Scaling your workload based on relevant business metrics such as HTTP requests, queue length, and cloud events can help reduce its resource utilization, hence its carbon emissions.

## Solution

Use [KEDA](https://keda.sh) when building event-driven kubernetes workloads, to allow scaling down to zero when there is no demand.

## SCI Impact
`SCI = (E * I) + M per R`
[Software Carbon Intensity Spec](https://grnsft.org/sci)

Regarding the SCI equation, scaling based on events will impact:

- `M`: By scaling the workloads based on demand and maximizing resource utilization, we reduce the total embodied carbon emissions by the kubernetes cluster.

## Assumptions

In addition to scaling kubernetes workloads based on events, cluster auto-scaling and bursting capabilities are used to maximize resource utilization.

## Considerations
If your workloads have predictable usage patterns, you could implement scaling based on time as a strategy to optimize utilization and reduce carbon emissions.