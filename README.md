# Prompts

This folder contains reusable AI prompts that support the daily workflow of a Software Engineer.

The prompts are technology-agnostic and can be used with:

* GitHub Copilot Chat
* GitHub Copilot Agent
* Cursor AI
* ChatGPT
* Claude
* Any AI coding assistant

---

## Folder Structure

```text
Prompts/
├── 01-requirement-analysis.md
├── 02-feature-implementation.md
├── 03-bug-fix.md
├── 04-code-analysis.md
└── 05-code-review.md
```

---

## 01 - Requirement Analysis

Purpose:

Analyze requirements before implementation.

Use this prompt to:

* Understand business requirements
* Identify business rules
* Identify validation rules
* Discover missing requirements
* Identify edge cases
* Generate acceptance criteria
* Clarify assumptions

Recommended Usage:

* New task
* User story refinement
* Requirement clarification
* Sprint planning

---

## 02 - Feature Implementation

Purpose:

Implement a new feature or enhancement using existing project patterns.

Use this prompt to:

* Analyze existing implementation
* Identify impacted files
* Understand dependencies
* Create implementation plans
* Generate code changes
* Minimize regression risk

Recommended Usage:

* New feature development
* Feature enhancement
* Change requests

---

## 03 - Bug Fix

Purpose:

Investigate and fix defects safely.

Use this prompt to:

* Perform root cause analysis
* Analyze affected flows
* Identify impacted files
* Assess regression risks
* Generate safe code changes
* Create verification steps

Recommended Usage:

* QA defects
* Development bugs
* Production issues
* Regression bugs

---

## 04 - Code Analysis

Purpose:

Understand existing code before making changes.

Use this prompt to:

* Understand component responsibilities
* Understand business flows
* Identify dependencies
* Discover hidden business logic
* Analyze current architecture
* Reduce onboarding time

Recommended Usage:

* Legacy code investigation
* New team onboarding
* Impact analysis
* Feature enhancement

---

## 05 - Code Review

Purpose:

Review implementation quality before merge.

Use this prompt to:

* Identify bugs
* Review business logic
* Review edge cases
* Review security concerns
* Review performance concerns
* Review maintainability
* Identify technical debt

Recommended Usage:

* Self-review
* Pull request review
* Pre-merge validation

---

## Recommended Workflow

### New Feature

1. 01-requirement-analysis.md
2. 04-code-analysis.md
3. 02-feature-implementation.md
4. 05-code-review.md
5. Testing
6. Pull Request

---

### Bug Fix

1. 03-bug-fix.md
2. 04-code-analysis.md
3. Fix Implementation
4. 05-code-review.md
5. Testing
6. Pull Request

---

### Existing Code Investigation

1. 04-code-analysis.md
2. Requirement Analysis
3. Implementation
4. Review

---

## Best Practices

* Always provide sufficient context.
* Include related requirements.
* Include relevant code snippets.
* Include logs and error messages when debugging.
* Ask AI to explain reasoning before generating code.
* Validate generated output before applying changes.
* Review all generated code before merging.

---

## Philosophy

AI should be used as an Engineering Assistant, not as a replacement for engineering judgment.

The engineer remains responsible for:

* Requirement understanding
* Architecture decisions
* Code quality
* Security
* Testing
* Production readiness

```
```
