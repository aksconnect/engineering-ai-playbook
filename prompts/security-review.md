# 🔒 Security Review Playbook

## 🎯 Purpose

Use this playbook to perform a comprehensive security review of an application, service, API, or system before it reaches production.

Rather than scanning only for common vulnerabilities, this playbook evaluates the application's overall security posture, identifies risks, and recommends practical improvements with clear business and technical impact.

It is suitable for web, mobile, backend, cloud-native, and distributed systems.

---

# ✅ When to Use

Use this playbook when you want to:

* Review an application before release
* Perform a security assessment
* Review authentication and authorization
* Validate secure coding practices
* Identify potential vulnerabilities
* Review cloud security
* Review API security
* Prepare for penetration testing
* Improve overall security posture

---

# 📥 Inputs Required

Provide as much context as possible.

## Application Overview

Describe:

* What does the application do?
* Who are the users?
* What type of data is processed?

---

## Technology Stack

Examples:

* React
* Angular
* Flutter
* Node.js
* Spring Boot
* .NET
* PostgreSQL
* Redis
* Kubernetes
* AWS
* Azure

---

## Architecture

Provide:

* Architecture diagrams
* Authentication flow
* Deployment architecture
* Network topology
* API documentation

---

## Security Controls

Examples:

* Authentication mechanism
* Authorization model
* Encryption
* Secrets management
* Logging
* Monitoring
* Rate limiting

---

## Compliance Requirements

Examples:

* GDPR
* PCI-DSS
* HIPAA
* SOC2
* ISO 27001

---

## Known Concerns

List any existing security concerns or assumptions.

---

# 🚀 Copy-Paste Prompt

```text
Act as a Principal Security Architect performing a production readiness security review.

Your objective is to identify meaningful security risks, explain their impact, and recommend practical mitigations.

Avoid generic OWASP checklists unless they are directly relevant.

Use the following project context:

[Paste all available information here]

Review the application across the following dimensions.

## 1. Authentication

Review:

- Login flow
- MFA support
- Session management
- Password handling
- Token management

---

## 2. Authorization

Evaluate:

- Role-based access
- Permission checks
- Resource ownership
- Privilege escalation risks

---

## 3. Data Protection

Review:

- Encryption in transit
- Encryption at rest
- Sensitive data exposure
- Personally identifiable information
- Secrets handling

---

## 4. API Security

Review:

- Input validation
- Output validation
- Rate limiting
- Authentication
- Authorization
- Error responses

---

## 5. Infrastructure Security

Review:

- Cloud configuration
- Container security
- Network segmentation
- Firewalls
- IAM policies

---

## 6. Secure Coding

Review:

- Injection risks
- XSS
- CSRF
- SSRF
- Deserialization
- File uploads
- Dependency usage

---

## 7. Observability

Review:

- Security logging
- Audit trails
- Monitoring
- Alerting
- Incident response readiness

---

## 8. Supply Chain

Review:

- Third-party dependencies
- Package vulnerabilities
- Secrets in repositories
- CI/CD security

---

## 9. Compliance

Review alignment with applicable security and compliance requirements.

---

For every issue identified provide:

Severity

Critical

High

Medium

Low

Description

Potential attack scenario

Business impact

Technical impact

Likelihood

Recommended mitigation

Implementation effort

Trade-offs

---

Finally provide:

1. Executive Summary

2. Top Security Risks

3. Quick Security Improvements

4. Long-Term Security Recommendations

5. Overall Security Score (1–10)

6. Production Readiness Recommendation
```

---

# 📤 Expected Output

A comprehensive security assessment including:

* Executive Summary
* Risk Analysis
* Vulnerability Assessment
* Business Impact
* Prioritized Recommendations
* Security Score
* Production Readiness Recommendation

---

# ⭐ Pro Tips

Provide as much architectural and operational context as possible.

Useful inputs include:

* Architecture diagrams
* Authentication flows
* API specifications
* Infrastructure diagrams
* Cloud configuration
* Security requirements
* Threat model
* Existing security controls

Security reviews are significantly more effective when the reviewer understands both the technical implementation and the business context.

---

# 🚧 Common Mistakes

❌ Treating security as only an application code problem.

❌ Ignoring infrastructure and deployment.

❌ Reviewing authentication while overlooking authorization.

❌ Forgetting third-party dependencies and supply chain risks.

❌ Assuming compliance automatically means the application is secure.

---

# 🔗 Related Playbooks

* Architecture Review
* System Design Review
* Performance Review
* Root Cause Analysis
* API Design Review

---

# ✅ Human Review Checklist

Before approving the application for production, ask yourself:

* [ ] Are authentication and authorization implemented correctly?
* [ ] Is sensitive data adequately protected?
* [ ] Are secrets stored and managed securely?
* [ ] Are APIs protected against common abuse scenarios?
* [ ] Are dependencies and infrastructure reviewed for security risks?
* [ ] Is meaningful security logging and monitoring in place?
* [ ] Have compliance requirements been considered where applicable?
* [ ] Would I be comfortable exposing this application to the public Internet?

---

## 📄 License

MIT
