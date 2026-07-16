# ⚛️ Frontend Architecture Review Playbook

## 🎯 Purpose

Use this playbook to review the architecture of a frontend application before or during implementation.

Unlike a general architecture review, this playbook focuses on frontend-specific concerns such as component composition, state management, rendering performance, accessibility, scalability, design systems, and developer experience.

It is suitable for React, Angular, Vue, Next.js, Remix, Flutter Web, and other modern frontend applications.

---

# ✅ When to Use

Use this playbook when you want to:

* Review a frontend architecture
* Evaluate a React or Angular application
* Validate component boundaries
* Improve maintainability
* Review state management
* Assess design system adoption
* Prepare for large-scale frontend development
* Identify architectural risks before implementation

---

# 📥 Inputs Required

Provide as much context as possible.

## Product Context

Describe:

* What problem does the application solve?
* Who are the users?
* Expected scale
* Device targets
* Browser support

---

## Technology Stack

Examples:

* React
* Angular
* Next.js
* Vue
* TypeScript
* Nx
* Module Federation
* Vite
* Storybook

---

## Architecture

Include:

* Folder structure
* Component hierarchy
* Routing
* State management
* Data flow
* Design system
* API integration approach

---

## Functional Requirements

Examples:

* Authentication
* Dashboards
* Forms
* Search
* Real-time updates
* Offline support

---

## Non-Functional Requirements

Examples:

* Performance
* Accessibility
* SEO
* Scalability
* Maintainability
* Internationalization

---

# 🚀 Copy-Paste Prompt

```text
Act as a Principal Frontend Architect performing a comprehensive architecture review.

Review the proposed frontend architecture with the goal of identifying maintainability, scalability, performance, accessibility, and developer experience improvements.

Use the following project context:

[Paste all available information here]

Evaluate the architecture across the following dimensions.

## 1. Component Architecture

Review:

- Component boundaries
- Reusability
- Separation of concerns
- Composition patterns
- Smart vs presentational components

---

## 2. State Management

Review:

- Local state
- Global state
- Server state
- State ownership
- Data flow
- State synchronization

Recommend whether the current approach is appropriate.

---

## 3. Routing & Navigation

Review:

- Route organization
- Lazy loading
- Nested routing
- Code splitting
- Navigation patterns

---

## 4. Performance

Review:

- Bundle size
- Rendering strategy
- Memoization
- Lazy loading
- Image optimization
- Hydration (if applicable)
- Caching opportunities

---

## 5. Accessibility

Review:

- Semantic HTML
- Keyboard navigation
- Screen reader support
- Focus management
- Color contrast
- ARIA usage

---

## 6. Design System

Review:

- Component consistency
- Token usage
- Theming
- Responsive behavior
- Reusable UI primitives

---

## 7. Developer Experience

Review:

- Folder structure
- Naming conventions
- Testing strategy
- Storybook usage
- Documentation
- Ease of onboarding

---

## 8. Scalability

Evaluate:

- Feature modularity
- Team scalability
- Microfrontend readiness (if applicable)
- Shared libraries
- Dependency management

---

For every issue identified provide:

- Severity (Critical, High, Medium, Low)
- Description
- Business impact
- Technical impact
- Recommendation
- Trade-offs

Finally provide:

1. Executive Summary

2. Architectural Strengths

3. Architectural Risks

4. Top 5 Improvements

5. Frontend Architecture Score (1–10)

6. Production Readiness Recommendation
```

---

# 📤 Expected Output

A structured frontend architecture assessment including:

* Executive Summary
* Component Architecture Review
* State Management Assessment
* Performance Review
* Accessibility Review
* Design System Assessment
* Scalability Analysis
* Prioritized Recommendations
* Overall Architecture Score

---

# ⭐ Pro Tips

Provide:

* Component hierarchy diagrams
* Folder structure
* Routing configuration
* State management approach
* Screenshots
* Storybook links
* Design system documentation

The richer the context, the more actionable the architectural recommendations.

---

# 🚧 Common Mistakes

❌ Putting business logic directly inside UI components.

❌ Using global state for local concerns.

❌ Ignoring accessibility until the end of development.

❌ Optimizing for today's features instead of future growth.

❌ Creating reusable components before identifying real reuse.

❌ Treating the design system as optional.

---

# 🔗 Related Playbooks

* Architecture Review
* Performance Review
* Pull Request Review
* API Design Review
* Security Review

---

# ✅ Human Review Checklist

Before approving the frontend architecture, ask yourself:

* [ ] Are component responsibilities clearly defined?
* [ ] Is state managed at the appropriate level?
* [ ] Can the architecture scale as new features are added?
* [ ] Have accessibility requirements been considered?
* [ ] Is the design system consistently applied?
* [ ] Will new team members find the project easy to navigate?
* [ ] Would I be comfortable maintaining this architecture for the next three years?

---

## 📄 License

MIT
