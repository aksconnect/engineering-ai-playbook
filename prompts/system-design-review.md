# 🏛️ System Design Review Playbook

## 🎯 Purpose

Use this playbook to review and improve a proposed system design before implementation begins.

This playbook helps identify scalability risks, architectural trade-offs, missing requirements, bottlenecks, and design improvements early in the software development lifecycle.

It is intended for software engineers, architects, tech leads, engineering managers, and engineering teams designing distributed systems or large-scale applications.

---

# ✅ When to Use

Use this playbook when you want to:

* Review a new system design
* Validate a proposed architecture
* Prepare for a design review meeting
* Evaluate design trade-offs
* Improve scalability
* Identify bottlenecks before implementation
* Prepare for System Design interviews
* Compare multiple design options

---

# 📥 Inputs Required

Provide as much context as possible.

## Problem Statement

Describe:

* What problem is being solved?
* Who are the users?
* Why is the system needed?

---

## Functional Requirements

Examples:

* Authentication
* Payments
* Search
* Notifications
* Reporting
* File Uploads

---

## Non-Functional Requirements

Examples:

* Scalability
* Availability
* Reliability
* Security
* Performance
* Cost
* Disaster Recovery
* Compliance

---

## Proposed Design

Include:

* Architecture diagrams
* Component diagrams
* Data flow
* Sequence diagrams
* Database schema
* API design
* Deployment architecture

---

## Technology Choices

Examples:

* Programming language
* Frameworks
* Databases
* Messaging systems
* Cloud provider
* Caching
* CDN

---

## Constraints

Examples:

* Budget
* Team size
* Timeline
* Existing systems
* Regulatory requirements
* Vendor restrictions

---

# 🚀 Copy-Paste Prompt

```text
Act as a Principal Software Architect conducting a formal System Design Review.

Review the proposed system as if it is about to enter implementation.

Do not redesign the system from scratch.

Instead, evaluate whether the proposed design is appropriate for the stated requirements and constraints.

Use the following project context:

[Paste all available information here]

Review the design across the following dimensions.

## 1. Problem Understanding

- Is the problem clearly defined?
- Are the requirements complete?
- Are any assumptions missing?

---

## 2. Functional Coverage

Review whether the proposed design satisfies all functional requirements.

Identify missing capabilities.

---

## 3. Scalability

Review:

- Horizontal scaling
- Vertical scaling
- Load distribution
- Statelessness
- Caching strategy
- Database scalability

---

## 4. Reliability & Resilience

Evaluate:

- High availability
- Failure handling
- Retry strategies
- Timeouts
- Circuit breakers
- Disaster recovery

---

## 5. Performance

Review:

- Latency
- Throughput
- Database access
- Network communication
- Background processing
- Caching opportunities

---

## 6. Security

Review:

- Authentication
- Authorization
- Data protection
- Secrets management
- Encryption
- OWASP considerations

---

## 7. Data Design

Review:

- Database selection
- Data model
- Indexing
- Consistency
- Transactions
- Partitioning
- Replication

---

## 8. Maintainability

Review:

- Separation of concerns
- Modularity
- Extensibility
- Code ownership
- Service boundaries
- Documentation

---

## 9. Cost

Identify:

- Expensive components
- Over-engineering
- Opportunities to simplify
- Infrastructure optimization

---

## 10. Future Growth

Evaluate whether the design can support:

- 10x users
- 10x traffic
- 10x data
- 10x engineering team

---

For every issue identified provide:

- Severity (Critical, High, Medium, Low)
- Explanation
- Business impact
- Technical impact
- Recommendation
- Trade-offs

Finally provide:

1. Executive Summary

2. Strengths

3. Weaknesses

4. Top 5 Risks

5. Top 5 Improvements

6. Overall Design Score (1–10)

7. Go / No-Go Recommendation for implementation
```

---

# 📤 Expected Output

A structured System Design Review containing:

* Executive Summary
* Design Assessment
* Scalability Review
* Security Review
* Performance Review
* Reliability Assessment
* Risk Analysis
* Recommendations
* Overall Design Score
* Go / No-Go Recommendation

---

# ⭐ Pro Tips

The best reviews happen when you provide:

* Architecture diagrams
* Functional requirements
* Non-functional requirements
* Scale expectations
* Constraints
* Existing systems
* Technology choices

The more complete the design context, the more actionable the review will be.

---

# 🚧 Common Mistakes

❌ Reviewing a design without understanding the business problem.

❌ Ignoring non-functional requirements.

❌ Optimizing only for today's scale.

❌ Choosing technologies without explaining the trade-offs.

❌ Focusing on implementation details instead of architectural decisions.

---

# 🔗 Related Playbooks

* Architecture Review
* Pull Request Review
* Performance Review
* Security Review
* API Design Review

---

# ✅ Human Review Checklist

Before approving the system design, ask yourself:

* [ ] Does the design solve the intended business problem?
* [ ] Are both functional and non-functional requirements addressed?
* [ ] Can the system scale to future demand?
* [ ] Are reliability and failure scenarios considered?
* [ ] Is the security model appropriate?
* [ ] Are technology choices justified by the requirements?
* [ ] Have trade-offs been documented?
* [ ] Would I be comfortable building and maintaining this system over the next several years?

---

## 📄 License

MIT
