# 🚀 Performance Review Playbook

## 🎯 Purpose

Use this playbook to identify performance bottlenecks across an application, service, API, or system.

Rather than making generic optimization suggestions, this playbook performs a structured performance review to identify measurable bottlenecks, explain their impact, and recommend improvements with clear trade-offs.

It is suitable for frontend, backend, mobile, cloud-native, and distributed systems.

---

# ✅ When to Use

Use this playbook when you want to:

* Investigate slow applications
* Improve frontend performance
* Optimize backend APIs
* Reduce latency
* Improve scalability
* Optimize database queries
* Reduce cloud costs
* Prepare for production traffic
* Improve user experience

---

# 📥 Inputs Required

Provide as much context as possible.

## Problem Statement

Describe:

* What feels slow?
* What performance goals are expected?
* Is the issue consistent or intermittent?

---

## Technology Stack

Examples:

* React
* Angular
* Flutter
* Java
* Spring Boot
* .NET
* Node.js
* PostgreSQL
* Redis
* Kafka
* Kubernetes
* AWS
* Azure

---

## Performance Data

Include:

* Lighthouse reports
* Chrome DevTools
* Network traces
* Profiling data
* Flame graphs
* Memory snapshots
* CPU usage
* Database execution plans
* Monitoring dashboards

---

## Architecture

Provide:

* Architecture diagram
* Data flow
* Deployment topology
* Caching strategy
* Database design

---

## Scale

Examples:

* Concurrent users
* Requests per second
* Dataset size
* Traffic patterns

---

## Constraints

Examples:

* Budget
* Existing infrastructure
* Team size
* Timeline
* Technology limitations

---

# 🚀 Copy-Paste Prompt

```text
Act as a Principal Performance Engineer conducting a comprehensive performance review.

Your objective is not simply to suggest optimizations.

Instead, identify measurable bottlenecks, explain why they exist, prioritize them, and recommend improvements with clear trade-offs.

Use the following context:

[Paste project information here]

Review the application across the following dimensions.

## 1. User Experience

Review:

- Page load time
- Time to Interactive
- Rendering
- Responsiveness
- Mobile experience

---

## 2. Frontend Performance

Evaluate:

- Bundle size
- Rendering
- Re-renders
- Lazy loading
- Code splitting
- Image optimization
- Asset loading
- Memory usage

---

## 3. Backend Performance

Review:

- API latency
- Request handling
- Thread utilization
- Serialization
- Background processing

---

## 4. Database

Review:

- Query performance
- Indexes
- N+1 queries
- Transactions
- Locking
- Connection pooling

---

## 5. Network

Review:

- Payload sizes
- Compression
- CDN
- Caching headers
- HTTP versions
- Request waterfalls

---

## 6. Infrastructure

Review:

- Scaling
- Resource utilization
- Autoscaling
- Load balancing
- Storage
- Containers

---

## 7. Observability

Review:

- Logging
- Metrics
- Distributed tracing
- Profiling
- Alerting

---

## 8. Cost vs Performance

Identify:

- Expensive optimizations
- Low-cost improvements
- Quick wins
- Long-term investments

---

For every issue identified provide:

Severity:

Critical

High

Medium

Low

Current impact

Evidence

Root cause

Recommendation

Expected improvement

Trade-offs

Implementation complexity

---

Finally provide:

1. Executive Summary

2. Top 10 Bottlenecks

3. Quick Wins

4. Long-Term Optimizations

5. Performance Score (1–10)

6. Prioritized Action Plan
```

---

# 📤 Expected Output

A comprehensive performance assessment including:

* Executive Summary
* Performance bottlenecks
* Evidence-based analysis
* Prioritized recommendations
* Quick wins
* Long-term improvements
* Performance score

---

# ⭐ Pro Tips

Provide evidence whenever possible.

Examples include:

* Profiling results
* Network traces
* Lighthouse reports
* Database query plans
* Monitoring dashboards
* Performance metrics

Avoid asking AI to optimize code without explaining the performance problem you're trying to solve.

---

# 🚧 Common Mistakes

❌ Optimizing before measuring.

❌ Assuming the slowest function is the real bottleneck.

❌ Ignoring network latency.

❌ Ignoring database performance.

❌ Optimizing microseconds while ignoring user experience.

❌ Focusing only on CPU instead of the complete request lifecycle.

---

# 🔗 Related Playbooks

* Architecture Review
* System Design Review
* Root Cause Analysis
* Pull Request Review
* Security Review

---

# ✅ Human Review Checklist

Before implementing performance optimizations, ask yourself:

* [ ] Have we measured the problem rather than guessed?
* [ ] Is the bottleneck supported by evidence?
* [ ] Will users actually notice the improvement?
* [ ] Are we optimizing the correct layer (frontend, backend, database, or infrastructure)?
* [ ] Are the proposed optimizations worth their complexity?
* [ ] Have we considered scalability as well as latency?
* [ ] Will these optimizations remain valuable as the system grows?
* [ ] Have we defined how success will be measured after the changes?

---

## 📄 License

MIT
