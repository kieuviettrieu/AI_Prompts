# AI Development Workflow

This document describes how the prompts can be integrated into a Software Engineer's daily development workflow.

---

# New Feature Development Workflow

Use this workflow when implementing a new feature.

```text
01 Requirement Analysis
        ↓
04 Code Analysis
        ↓
02 Feature Implementation
        ↓
06 Test and Risk Analysis
        ↓
07 Self Review and Fix
        ↓
05 Code Review
        ↓
Create Pull Request
        ↓
QA Testing
```

---

## Step 1: Requirement Analysis

Prompt:

```text
01-requirement-analysis.md
```

Goal:

* Understand business requirements
* Identify business rules
* Identify validation requirements
* Discover edge cases
* Clarify ambiguous requirements

Output:

* Requirement breakdown
* Business rules
* Validation rules
* Acceptance criteria
* Clarification questions
* Risks

---

## Step 2: Code Analysis

Prompt:

```text
04-code-analysis.md
```

Goal:

* Understand existing implementation
* Understand business flow
* Identify related modules
* Identify impacted components

Output:

* Existing execution flow
* Business logic flow
* Dependencies
* Impacted areas

---

## Step 3: Feature Implementation

Prompt:

```text
02-feature-implementation.md
```

Goal:

* Implement the requirement
* Follow existing architecture
* Minimize impact on existing behavior

Output:

* Implementation plan
* Code changes
* Risks
* Test recommendations

---

## Step 4: Test and Risk Analysis

Prompt:

```text
06-test-and-risk-analysis.md
```

Goal:

* Validate implementation coverage
* Identify missing scenarios
* Identify edge cases
* Identify potential bugs before QA

Output:

* Requirement gaps
* Missing validations
* Missing scenarios
* Risk analysis

---

## Step 5: Self Review and Fix

Prompt:

```text
07-self-review-and-fix.md
```

Goal:

* Perform self-review
* Resolve issues before PR
* Improve implementation quality

Output:

* Findings
* Safe fixes
* Regression verification
* Merge readiness

---

## Step 6: Code Review

Prompt:

```text
05-code-review.md
```

Goal:

* Perform final implementation review
* Identify remaining issues
* Verify readiness for peer review

Output:

* Review findings
* Risk assessment
* Merge recommendation

---

# Bug Fix Workflow

Use this workflow when fixing defects.

```text
03 Bug Fix
        ↓
06 Test and Risk Analysis
        ↓
07 Self Review and Fix
        ↓
05 Code Review
        ↓
Create Pull Request
```

---

# Existing Code Investigation Workflow

Use this workflow when working with unfamiliar code.

```text
04 Code Analysis
        ↓
Understand Existing Logic
        ↓
Implement Changes Safely
```

---

# How to Use

1. Select the prompt that matches your task.
2. Copy the prompt into your preferred AI assistant.
3. Provide sufficient context:

   * Requirement
   * Source code
   * Pull Request
   * Bug report
   * Related files
4. Review AI output critically.
5. Apply changes only after validation.

AI should support engineering decisions, not replace engineering judgment.
