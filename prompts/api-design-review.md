# 🌐 API Design Review Playbook

## 🎯 Purpose

Use this playbook to perform a comprehensive review of an API before implementation or public release.

Rather than reviewing only endpoint definitions, this playbook evaluates the API as a long-term contract between producers and consumers.

It helps identify usability issues, scalability concerns, security risks, versioning problems, and opportunities to improve developer experience.

Suitable for:

* REST APIs
* GraphQL APIs
* gRPC Services
* Internal APIs
* Public APIs
* Partner APIs

---

# ✅ When to Use

Use this playbook when you want to:

* Review a new API design
* Validate an existing API
* Prepare for implementation
* Improve developer experience
* Review versioning strategy
* Improve API consistency
* Identify breaking changes
* Prepare for production release

---

# 📥 Inputs Required

Provide as much context as possible.

## Business Context

Describe:

* What problem does the API solve?
* Who are the consumers?
* Internal or public API?
* Expected traffic

---

## API Specification

Include:

* OpenAPI / Swagger specification
* GraphQL schema
* Endpoint definitions
* Request examples
* Response examples

---

## Functional Requirements

Examples:

* Authentication
* Search
* Pagination
* Bulk operations
* File uploads
* Notifications

---

## Non-Functional Requirements

Examples:

* Scalability
* Performance
* Security
* Availability
* Backward compatibility
* Rate limits

---

## Constraints

Examples:

* Existing consumers
* Legacy integrations
* Compliance
* Infrastructure limitations

---

# 🚀 Copy-Paste Prompt

```text
Act as a Principal API Architect performing a production-quality API Design Review.

Your objective is to evaluate the API as a long-term contract between producers and consumers.

Avoid focusing only on endpoint syntax.

Instead, review the API for usability, consistency, scalability, security, maintainability, and developer experience.

Use the following project context:

[Paste all available information here]

Review the API across the following dimensions.

## 1. API Design

Review:

- Resource modeling
- Naming conventions
- URI structure
- HTTP method usage
- Consistency

---

## 2. Request & Response Design

Review:

- Payload structure
- Field naming
- Validation
- Optional fields
- Default values

---

## 3. Error Handling

Review:

- HTTP status codes
- Error messages
- Error format
- Validation responses
- Retry guidance

---

## 4. Versioning

Review:

- Versioning strategy
- Backward compatibility
- Deprecation approach
- Breaking changes

---

## 5. Performance

Review:

- Pagination
- Filtering
- Sorting
- Field selection
- Payload size
- Batch operations

---

## 6. Security

Review:

- Authentication
- Authorization
- Rate limiting
- Sensitive data exposure
- Input validation

---

## 7. Developer Experience

Review:

- API discoverability
- Documentation quality
- Example requests
- SDK friendliness
- Ease of integration

---

## 8. Observability

Review:

- Logging
- Correlation IDs
- Traceability
- Monitoring
- Auditability

---

## 9. Scalability

Evaluate:

- Future endpoints
- API evolution
- Consumer growth
- Traffic growth

---

For every issue identified provide:

Severity

Critical

High

Medium

Low

Description

Business impact

Technical impact

Recommendation

Trade-offs

---

Finally provide:

1. Executive Summary

2. Strengths

3. Weaknesses

4. Top 5 Design Risks

5. Top 5 Improvements

6. API Design Score (1–10)

7. Production Readiness Recommendation
```

---

# 📤 Expected Output

A structured API design review containing:

* Executive Summary
* API Design Assessment
* Developer Experience Review
* Security Review
* Performance Review
* Versioning Assessment
* Scalability Assessment
* Prioritized Recommendations
* Overall API Design Score

---

# ⭐ Pro Tips

Whenever possible, provide:

* OpenAPI specification
* Sample requests and responses
* Authentication flow
* Consumer expectations
* Error response examples
* Performance requirements

The more complete the API specification, the more actionable the review.

---

# 🚧 Common Mistakes

❌ Designing APIs around database tables instead of business resources.

❌ Ignoring versioning until after release.

❌ Returning inconsistent error formats.

❌ Forgetting pagination, filtering, and sorting.

❌ Exposing implementation details through the API.

❌ Optimizing for today's consumers instead of future growth.

---

# 🔗 Related Playbooks

* Architecture Review
* System Design Review
* Security Review
* Performance Review
* Pull Request Review

---

# ✅ Human Review Checklist

Before approving the API design, ask yourself:

* [ ] Is the API intuitive for consumers?
* [ ] Are naming conventions consistent?
* [ ] Are request and response models easy to understand?
* [ ] Is error handling consistent and helpful?
* [ ] Does the versioning strategy support future evolution?
* [ ] Are security considerations addressed?
* [ ] Can the API scale with future consumers and traffic?
* [ ] Would I enjoy integrating with this API as a developer?

---

## 📄 License

MIT
