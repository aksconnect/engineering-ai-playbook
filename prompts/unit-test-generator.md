# 🧪 Unit Test Generator Playbook

## 🎯 Purpose

Use this playbook to generate high-quality, maintainable unit tests that validate behavior, edge cases, and error handling—not just improve code coverage.

This playbook is designed for software engineers who want AI to generate production-quality tests that are readable, reliable, and easy to maintain.

---

# ✅ When to Use

Use this playbook when you want to:

* Generate unit tests for new code
* Improve existing test coverage
* Add regression tests
* Validate bug fixes
* Generate edge case tests
* Improve confidence before refactoring
* Review existing unit tests

---

# 📥 Inputs Required

Provide as much context as possible.

## Source Code

Include:

* Function
* Class
* Component
* Service
* Hook
* Utility

---

## Business Purpose

Explain:

* What problem does this code solve?
* What should happen?
* What should never happen?

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

---

## Testing Framework

Examples:

* Jest
* Vitest
* JUnit
* NUnit
* xUnit
* Flutter Test
* Playwright (for component tests)

---

## Existing Tests (Optional)

Provide current test cases if available.

---

## Known Edge Cases

Examples:

* Empty input
* Null values
* Invalid IDs
* Network failures
* Timeouts
* Duplicate data

---

# 🚀 Copy-Paste Prompt

```text
Act as a Senior Software Engineer with extensive experience writing maintainable unit tests.

Generate production-quality unit tests for the following code.

Do not simply maximize code coverage.

Instead, create tests that validate the intended behavior of the software.

Use the following context:

[Paste business context]

[Paste source code]

[Paste testing framework]

Review the implementation and generate tests covering the following.

## 1. Happy Path

Verify the expected behavior under normal conditions.

---

## 2. Edge Cases

Identify and test:

- Empty values
- Null values
- Boundary conditions
- Invalid input
- Duplicate values

---

## 3. Error Handling

Verify:

- Exceptions
- Validation failures
- Unexpected input
- Failure scenarios

---

## 4. Business Rules

Ensure all business rules are verified.

If any business rules are unclear, identify them.

---

## 5. Test Quality

Ensure tests are:

- Readable
- Independent
- Deterministic
- Easy to maintain
- Properly named

Avoid brittle or implementation-specific tests.

---

## 6. Missing Test Scenarios

Identify important scenarios that are currently untested.

Explain why they matter.

---

## 7. Refactoring Opportunities

If the code is difficult to test:

- Explain why
- Suggest improvements
- Recommend dependency injection, abstractions, or design changes where appropriate

---

Finally provide:

1. Complete unit test implementation

2. Coverage Summary

3. Untested Risks

4. Suggested Refactoring (if applicable)

5. Confidence Assessment
```

---

# 📤 Expected Output

A comprehensive testing package containing:

* Complete unit tests
* Happy path tests
* Edge case tests
* Error handling tests
* Missing scenario analysis
* Refactoring recommendations
* Coverage summary

---

# ⭐ Pro Tips

Provide:

* Business requirements
* Existing tests
* Testing framework
* Expected behavior
* Known bugs
* Edge cases

The more context you provide, the better the generated tests will reflect the actual intent of the code.

---

# 🚧 Common Mistakes

❌ Asking for tests without providing the implementation.

❌ Optimizing only for code coverage.

❌ Ignoring business rules.

❌ Writing tests that depend on implementation details rather than observable behavior.

❌ Forgetting edge cases and failure scenarios.

---

# 🔗 Related Playbooks

* Pull Request Review
* Root Cause Analysis
* Architecture Review
* Performance Review
* System Design Review

---

# ✅ Human Review Checklist

Before accepting generated tests, ask yourself:

* [ ] Do the tests verify business behavior instead of implementation details?
* [ ] Are important edge cases covered?
* [ ] Are failure scenarios tested?
* [ ] Are test names descriptive?
* [ ] Are the tests independent and deterministic?
* [ ] Will these tests remain valuable after refactoring?
* [ ] Would these tests help prevent regressions?

---

## 📄 License

MIT
