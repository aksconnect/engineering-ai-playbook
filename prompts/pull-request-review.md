# 🔍 Pull Request Review Playbook

## 🎯 Purpose

Use this playbook to perform a comprehensive review of a Pull Request (PR) before merging it into the main branch.

Unlike a standard code review, this playbook evaluates the PR through multiple engineering lenses—including correctness, architecture, performance, security, maintainability, testing, and long-term impact.

The goal is not simply to find issues, but to improve the overall quality of the software.

---

# ✅ When to Use

Use this playbook when you want to:

* Review a Pull Request before merging
* Perform a self-review before requesting reviewers
* Improve code quality
* Reduce technical debt
* Identify hidden risks
* Validate architectural decisions
* Mentor junior engineers
* Ensure production readiness

---

# 📥 Inputs Required

Provide as much context as possible.

## Business Context

* What problem is this PR solving?
* Why is this change required?
* Who benefits from it?

---

## Pull Request Description

Include:

* PR summary
* Acceptance criteria
* Linked ticket (Jira, Azure DevOps, GitHub Issue, etc.)
* Screenshots (if UI changes)

---

## Technology Stack

Examples:

* React
* Angular
* Flutter
* Node.js
* Java
* .NET
* Spring Boot

---

## Code Changes

Include:

* Files changed
* Key classes/components
* Relevant code snippets or full diff
* Configuration changes

---

## Constraints

Examples:

* Performance requirements
* Browser support
* Mobile compatibility
* Accessibility requirements
* Release deadlines

---

# 🚀 Copy-Paste Prompt

```text
Act as a Principal Software Engineer performing a production-quality Pull Request review.

Review the following Pull Request.

Do not focus only on syntax or style.

Review the change as if it will be deployed to production tomorrow.

Use the following project context:

[Paste project context here]

Use the following PR information:

[Paste PR description, code diff, screenshots, and related ticket]

Evaluate the Pull Request across the following dimensions.

## 1. Functional Correctness

- Does the implementation solve the stated problem?
- Are there hidden bugs?
- Are edge cases handled?
- Are there regressions?

---

## 2. Architecture

Review:

- Separation of concerns
- Coupling
- Cohesion
- Layering
- Reusability
- Design patterns
- Long-term maintainability

---

## 3. Code Quality

Review:

- Naming
- Readability
- Complexity
- Duplication
- SOLID principles
- Code smells

---

## 4. Performance

Review:

- Rendering performance
- Database/API efficiency
- Unnecessary computations
- Memory usage
- Network calls
- Lazy loading opportunities

---

## 5. Security

Review:

- Authentication
- Authorization
- Sensitive data
- Secrets
- Injection risks
- OWASP concerns
- Input validation

---

## 6. Testing

Review:

- Unit tests
- Integration tests
- Edge cases
- Missing test scenarios
- Test quality

---

## 7. Accessibility (if applicable)

Review:

- Keyboard navigation
- Screen readers
- Color contrast
- Semantic HTML
- ARIA usage

---

## 8. Developer Experience

Review:

- Documentation
- Comments
- Discoverability
- Configuration
- Future maintenance

---

## 9. Breaking Changes

Identify:

- API changes
- Database changes
- Migration requirements
- Backward compatibility concerns

---

## 10. Production Readiness

Would you approve this PR for production deployment?

Explain why.

---

For every issue found provide:

Severity:

Critical

High

Medium

Low

Description

Why it matters

Suggested improvement

Example implementation (where appropriate)

Trade-offs

Finally provide:

1. Executive Summary

2. Approval Recommendation

Approve

Approve with Minor Changes

Request Changes

Reject

3. Top Risks

4. Positive Observations

5. Technical Debt Introduced

6. Suggested Follow-up Tasks

7. Overall PR Score (1–10)
```

---

# 📤 Expected Output

A comprehensive Pull Request review containing:

* Executive Summary
* Approval Recommendation
* Prioritized issues
* Strengths
* Risks
* Suggested improvements
* Production readiness assessment

---

# ⭐ Pro Tips

The quality of the review depends heavily on the context you provide.

Include:

* The business problem
* The full PR description
* The code diff
* Screenshots (for UI changes)
* Related tickets
* Constraints
* Existing architecture

The richer the context, the more actionable and relevant the review will be.

---

# 🚧 Common Mistakes

❌ Reviewing only the changed lines without understanding the surrounding architecture.

❌ Omitting the business context.

❌ Providing only screenshots instead of the actual code diff.

❌ Ignoring edge cases and regression risks.

❌ Focusing solely on code style instead of long-term maintainability.

---

# 🔗 Related Playbooks

* Architecture Review
* Root Cause Analysis
* Performance Review
* Security Review
* Unit Test Generator
* System Design Review

---

## 📄 License

MIT
