# 🧠 State Management Review Playbook

## 🎯 Purpose

Use this playbook to review how application state is modeled, owned, shared, updated, and maintained.

This playbook helps identify unnecessary complexity, duplicated state, synchronization issues, performance problems, and opportunities to simplify data flow.

It applies to modern frontend frameworks including React, Angular, Vue, Flutter, and mobile applications.

---

# ✅ When to Use

Use this playbook when you want to:

* Review application state management
* Refactor a growing application
* Reduce unnecessary complexity
* Improve rendering performance
* Eliminate duplicated state
* Simplify data flow
* Evaluate state management libraries
* Prepare for large-scale frontend development

---

# 📥 Inputs Required

Provide as much context as possible.

## Application Overview

Describe:

* What does the application do?
* Primary user workflows
* Major screens
* Expected scale

---

## Technology Stack

Examples:

* React
* Angular
* Vue
* Flutter
* Next.js
* TypeScript

---

## Current State Management

Examples:

* React Context
* Redux Toolkit
* Zustand
* MobX
* NgRx
* Angular Signals
* RxJS
* Riverpod
* Provider
* Bloc

---

## Application Architecture

Provide:

* Folder structure
* Component hierarchy
* State ownership
* Data flow diagrams
* API interaction

---

## Known Problems

Examples:

* Too many re-renders
* Difficult debugging
* Synchronization issues
* Complex reducers
* Large stores
* Circular dependencies

---

# 🚀 Copy-Paste Prompt

```text
Act as a Principal Frontend Architect specializing in state management.

Review the application's state management strategy.

Your objective is not to recommend a different state library.

Instead, evaluate whether state is owned, updated, synchronized, and consumed appropriately.

Use the following project context:

[Paste project information here]

Review the application across the following dimensions.

## 1. State Ownership

Review:

- Local state
- Shared state
- Global state
- Server state

Determine whether each piece of state lives at the appropriate level.

---

## 2. Data Flow

Review:

- One-way data flow
- State synchronization
- Derived state
- Prop drilling
- Event communication

---

## 3. State Duplication

Identify:

- Duplicate state
- Derived state stored unnecessarily
- Cached data duplication
- Multiple sources of truth

---

## 4. Performance

Review:

- Unnecessary re-renders
- Selector efficiency
- Memoization
- Change detection
- Observable subscriptions
- Signal updates

---

## 5. State Organization

Review:

- Store structure
- Feature boundaries
- Module ownership
- Separation of concerns

---

## 6. Server State

Review:

- API caching
- Optimistic updates
- Synchronization
- Retry strategies
- Loading states
- Error handling

---

## 7. Scalability

Evaluate whether the state architecture can support:

- More developers
- More features
- More screens
- Offline support
- Real-time updates

---

For every issue identified provide:

Severity

Critical

High

Medium

Low

Description

Root Cause

Business Impact

Technical Impact

Recommendation

Trade-offs

---

Finally provide:

1. Executive Summary

2. Current State Assessment

3. Top Risks

4. Simplification Opportunities

5. Performance Improvements

6. Overall State Management Score (1–10)

7. Long-Term Recommendation
```

---

# 📤 Expected Output

A comprehensive review containing:

* Executive Summary
* State Ownership Analysis
* Data Flow Review
* Performance Assessment
* Scalability Assessment
* Simplification Opportunities
* Overall Score
* Prioritized Recommendations

---

# ⭐ Pro Tips

Include:

* Component hierarchy
* Store structure
* API flow
* Folder organization
* State management library
* Screenshots of complex workflows
* Existing performance concerns

The more context you provide, the more practical the recommendations.

---

# 🚧 Common Mistakes

❌ Putting everything into global state.

❌ Storing derived data instead of calculating it.

❌ Having multiple sources of truth.

❌ Mixing UI state with business state.

❌ Synchronizing state manually across multiple components.

❌ Optimizing with memoization before understanding the data flow.

---

# 🔗 Related Playbooks

* Frontend Architecture Review
* Performance Review
* Pull Request Review
* API Design Review
* Unit Test Generator

---

# ✅ Human Review Checklist

Before approving the state management approach, ask yourself:

* [ ] Does every piece of state have a clear owner?
* [ ] Is there a single source of truth for important data?
* [ ] Are UI state and business state clearly separated?
* [ ] Are unnecessary re-renders minimized?
* [ ] Is server state managed differently from client state?
* [ ] Will this architecture remain understandable as the application grows?
* [ ] Could a new engineer quickly understand the application's data flow?

---

## 📄 License

MIT
