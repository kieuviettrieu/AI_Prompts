# Prompt Guide

This document explains the purpose and recommended usage of each prompt.

---

# 01 - Requirement Analysis

File:

```text
01-requirement-analysis.md
```

Purpose:

Analyze requirements before implementation begins.

When to Use:

* New features
* User stories
* Change requests
* Requirement refinement

Output:

* Requirement summary
* Business rules
* Validation rules
* User flows
* Acceptance criteria
* Edge cases
* Risks

---

# 02 - Feature Implementation

File:

```text
02-feature-implementation.md
```

Purpose:

Implement new functionality while following existing project patterns.

When to Use:

* Feature development
* Enhancements
* Requirement implementation

Output:

* Impact analysis
* Implementation plan
* Code changes
* Risks
* Test recommendations

---

# 03 - Bug Fix

File:

```text
03-bug-fix.md
```

Purpose:

Investigate and fix defects safely.

When to Use:

* Functional bugs
* Validation bugs
* Logic bugs
* Production defects

Output:

* Root cause analysis
* Fix strategy
* Code changes
* Verification steps

---

# 04 - Code Analysis

File:

```text
04-code-analysis.md
```

Purpose:

Understand existing code and business logic.

When to Use:

* New project onboarding
* Existing feature investigation
* Legacy code analysis

Output:

* Architecture overview
* Business flow
* Execution flow
* Dependencies

---

# 05 - Code Review

File:

```text
05-code-review.md
```

Purpose:

Review implementation quality before opening a Pull Request.

When to Use:

* Before PR creation
* Before peer review
* Before code handoff

Output:

* Logic findings
* Missing scenarios
* Code quality findings
* Regression risks

---

# 06 - Test and Risk Analysis

File:

```text
06-test-and-risk-analysis.md
```

Purpose:

Identify requirement gaps, missing scenarios, validations, and risks before QA.

When to Use:

* After development
* Before QA testing
* Before UAT

Output:

* Missing requirements
* Missing validations
* Edge cases
* Potential bugs
* Risk assessment

---

# 07 - Self Review and Fix

File:

```text
07-self-review-and-fix.md
```

Purpose:

Perform a complete self-review and improvement cycle.

When to Use:

* Before Pull Request
* Before code review
* Before QA handoff

Output:

* Findings
* Safe fixes
* Verification results
* Merge readiness

---

# Recommended Usage

For most development tasks:

```text
01 → 04 → 02 → 06 → 07 → 05
```

For bug fixes:

```text
03 → 06 → 07 → 05
```

For understanding code:

```text
04
```
