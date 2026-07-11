# 🏗 Architecture Review Playbook

## 🎯 Purpose

Use this playbook to perform a comprehensive review of a software system's architecture.

It is designed for software engineers, architects, tech leads, engineering managers, and engineering teams who want AI to provide actionable architectural feedback rather than generic suggestions.

This playbook works well for:

* Greenfield projects
* Existing applications
* Microservices
* Monoliths
* Frontend applications
* Mobile applications
* Cloud-native systems
* AI-powered applications

---

# ✅ When to Use

Use this playbook when you want to:

* Review an existing architecture
* Design a new system
* Validate architectural decisions
* Identify scalability risks
* Improve maintainability
* Reduce technical debt
* Prepare for production
* Review another team's design
* Prepare for an architecture review meeting

---

# 📥 Inputs Required

Provide as much context as possible.

## Business Context

* What problem does the system solve?
* Who are the users?
* Expected traffic
* Business priorities

---

## Technology Stack

Example:

* React
* Flutter
* Angular
* Spring Boot
* .NET
* Node.js
* PostgreSQL
* MongoDB
* Redis
* Kafka
* Kubernetes
* AWS
* Azure

---

## Current Architecture

Provide:

* Architecture diagram
* Folder structure
* Deployment diagram
* Component diagram
* Service boundaries

---

## Functional Requirements

Examples:

* Authentication
* Payments
* Search
* Reporting
* Notifications

---

## Non-Functional Requirements

Examples:

* Performance
* Scalability
* Security
* Availability
* Disaster Recovery
* Cost
* Accessibility
* Compliance

---

## Constraints

Examples:

* Budget
* Timeline
* Existing technology
* Team size
* Cloud provider
* Regulatory requirements

---

## Current Pain Points

Examples:

* Slow builds
* High latency
* Difficult deployments
* Poor developer experience
* Memory issues
* Tight coupling

---

# 🚀 Copy-Paste Prompt

```text
Act as a Principal Software Architect with experience designing and reviewing enterprise-scale systems.

Review the following software architecture.

Do not provide generic recommendations.

Instead, perform a production-quality architecture review.

Use the following context:

[Paste all project information here]

Please review the architecture across the following dimensions.

## Business Alignment

- Does the architecture support the business goals?
- Is it unnecessarily complex?
- Are there missing capabilities?

---

## Scalability

Review:

- Horizontal scalability
- Vertical scalability
- Bottlenecks
- Statelessness
- Resource utilization

---

## Reliability

Evaluate:

- Fault tolerance
- Retry strategies
- Circuit breakers
- Timeouts
- Recovery
- Resilience

---

## Performance

Review:

- Network calls
- Rendering
- Database access
- Caching
- Lazy loading
- Background processing

---

## Maintainability

Review:

- Separation of concerns
- Coupling
- Cohesion
- Module boundaries
- Naming
- Folder structure

---

## Security

Review:

- Authentication
- Authorization
- Secrets
- Sensitive data
- OWASP concerns
- Encryption

---

## Observability

Review:

- Logging
- Monitoring
- Metrics
- Tracing
- Alerting

---

## Developer Experience

Review:

- Local development
- CI/CD
- Testing
- Documentation
- Onboarding

---

## Cost

Identify:

- Expensive infrastructure
- Over-engineering
- Opportunities to simplify

---

## Future Growth

Review whether the architecture will continue to work for:

10x users

10x engineers

10x traffic

---

For every issue found provide:

- Severity (Critical, High, Medium, Low)
- Explanation
- Business impact
- Technical impact
- Recommended solution
- Trade-offs
- Priority

Finally provide:

1. Executive Summary

2. Top 5 Risks

3. Top 5 Improvements

4. Technical Debt Assessment

5. Overall Architecture Score (1-10)

6. Suggested Next Steps
```

---

# 📤 Expected Output

A high-quality architecture review containing:

* Executive Summary
* Architecture Score
* Risks
* Opportunities
* Technical Debt
* Scalability Assessment
* Security Assessment
* Performance Assessment
* Prioritized Recommendations

---

# ⭐ Pro Tips

The quality of the review depends heavily on the quality of the context you provide.

Instead of asking:

> Review my architecture.

Provide:

* Architecture diagrams
* Business goals
* Non-functional requirements
* Existing pain points
* Expected scale
* Technology stack
* Team constraints

The richer the context, the more practical and actionable the recommendations will be.

---

# 🚧 Common Mistakes

❌ Only sharing code without explaining the business problem.

❌ Forgetting non-functional requirements.

❌ Not explaining deployment architecture.

❌ Asking for "best architecture" without defining constraints.

❌ Omitting current pain points.

---

# 🔗 Related Playbooks

* Pull Request Review
* System Design Review
* Root Cause Analysis
* Performance Review
* Security Review

---

## 📄 License

MIT
