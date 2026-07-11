# 🐞 Root Cause Analysis Playbook

## 🎯 Purpose

Use this playbook to systematically investigate bugs, production incidents, failures, regressions, performance issues, and unexpected system behavior.

Rather than jumping to conclusions or proposing immediate fixes, this playbook helps identify the true root cause, assess impact, and recommend corrective and preventive actions.

---

# ✅ When to Use

Use this playbook when you want to:

* Investigate a production incident
* Debug a difficult bug
* Analyze performance degradation
* Understand intermittent failures
* Investigate application crashes
* Perform post-incident reviews
* Identify regression causes
* Prepare an RCA document

---

# 📥 Inputs Required

Provide as much context as possible.

## Problem Summary

Describe:

* What happened?
* What was expected?
* What actually occurred?

---

## Timeline

Include:

* When did the issue begin?
* Was it after a deployment?
* Was it intermittent or consistent?
* Has it happened before?

---

## Environment

Examples:

* Development
* QA
* Staging
* Production

Include:

* OS
* Browser
* Device
* Cloud provider
* Region (if applicable)

---

## Technical Context

Provide:

* Technology stack
* Architecture overview
* Recent deployments
* Recent configuration changes
* Relevant code snippets

---

## Evidence

Include:

* Error logs
* Stack traces
* Screenshots
* Monitoring graphs
* Metrics
* Console output
* Network traces

---

## Reproduction Steps

If known:

* Steps to reproduce
* Frequency
* Preconditions

---

# 🚀 Copy-Paste Prompt

```text
Act as a Principal Software Engineer leading a production incident investigation.

Your objective is NOT to guess the answer.

Your objective is to determine the most probable root cause using evidence.

Use the following context:

[Paste all available information here]

Perform a structured Root Cause Analysis.

## 1. Problem Understanding

Summarize:

- What happened?
- Expected behavior
- Actual behavior

---

## 2. Evidence Review

Review all available:

- Logs
- Stack traces
- Metrics
- Screenshots
- Network traces
- Configuration
- Recent deployments

Identify observations without making assumptions.

---

## 3. Possible Causes

List every plausible root cause.

For each cause provide:

- Supporting evidence
- Contradicting evidence
- Confidence level (High / Medium / Low)

---

## 4. Root Cause

Identify the most probable root cause.

Explain:

- Why this is the most likely explanation
- Why alternative causes were rejected

---

## 5. Impact Assessment

Evaluate:

- Users affected
- Business impact
- Technical impact
- Severity
- Scope

---

## 6. Corrective Actions

Recommend:

- Immediate fixes
- Short-term improvements
- Long-term preventive measures

---

## 7. Prevention

Recommend improvements to prevent recurrence, including:

- Better monitoring
- Logging
- Testing
- Alerts
- Documentation
- Process improvements

---

## 8. Lessons Learned

Summarize:

- What the team should learn
- What should change going forward

---

Finally provide:

1. Executive Summary

2. Timeline of Events

3. Most Probable Root Cause

4. Confidence Level

5. Immediate Next Steps

6. Long-Term Recommendations
```

---

# 📤 Expected Output

A structured Root Cause Analysis report containing:

* Executive Summary
* Timeline
* Evidence Review
* Possible Causes
* Most Probable Root Cause
* Impact Assessment
* Corrective Actions
* Preventive Actions
* Lessons Learned

---

# ⭐ Pro Tips

The quality of the analysis depends on the evidence you provide.

Whenever possible, include:

* Logs
* Stack traces
* Monitoring metrics
* Deployment history
* Configuration changes
* Error messages
* Reproduction steps

Avoid asking AI to diagnose issues from a single error message without additional context.

---

# 🚧 Common Mistakes

❌ Assuming the first error message is the root cause.

❌ Ignoring recent deployments or configuration changes.

❌ Focusing only on application code while overlooking infrastructure, networking, or third-party dependencies.

❌ Providing conclusions instead of evidence.

❌ Jumping directly to solutions without validating the actual cause.

---

# 🔗 Related Playbooks

* Architecture Review
* Pull Request Review
* Performance Review
* Security Review
* System Design Review

---

# ✅ Human Review Checklist

Before accepting the root cause analysis, ask yourself:

* [ ] Have all available evidence been reviewed?
* [ ] Are conclusions supported by evidence rather than assumptions?
* [ ] Were multiple possible causes considered?
* [ ] Has the actual root cause been distinguished from symptoms?
* [ ] Is the business impact clearly understood?
* [ ] Have immediate corrective actions been identified?
* [ ] Have preventive actions been proposed?
* [ ] Would this analysis help prevent similar incidents in the future?

---

## 📄 License

MIT
