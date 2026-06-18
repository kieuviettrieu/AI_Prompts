# AI Prompts for Software Engineers

A collection of reusable AI prompts designed to support daily software engineering activities.

These prompts are technology-agnostic and can be used with:

- GitHub Copilot
- ChatGPT
- Claude
- Gemini
- Cursor
- Windsurf
- Any AI coding assistant

The goal is to improve:

- Requirement understanding
- Feature implementation quality
- Bug fixing efficiency
- Code review quality
- Risk identification
- Self-validation before QA
- Overall development productivity

---

# Prompt List

## 01 - Requirement Analysis

File:

```text
01-requirement-analysis.md
```

Purpose:

Analyze and break down requirements before implementation.

Output:

- Business requirements
- Business rules
- Validation rules
- Acceptance criteria
- Assumptions
- Missing requirements
- Edge cases
- Impact analysis

Recommended Usage:

Before starting any development task.

---

## 02 - Feature Implementation

File:

```text
02-feature-implementation.md
```

Purpose:

Implement new features following the existing codebase architecture and patterns.

Output:

- Requirement analysis
- Existing implementation analysis
- Impact analysis
- Edge cases
- Implementation plan
- Code changes
- Risks
- Test recommendations

Recommended Usage:

When developing new functionality.

---

## 03 - Bug Fix

File:

```text
03-bug-fix.md
```

Purpose:

Analyze and safely fix bugs while minimizing regression risk.

Output:

- Root cause analysis
- Existing flow analysis
- Risk assessment
- Fix strategy
- Code changes
- Verification steps
- Regression test recommendations

Recommended Usage:

When investigating and fixing defects.

---

## 04 - Code Analysis

File:

```text
04-code-analysis.md
```

Purpose:

Understand an existing component, module, feature, or business flow.

Output:

- Architecture overview
- Execution flow
- Business logic flow
- Validation flow
- Dependencies
- Data flow
- Potential risks

Recommended Usage:

When working with unfamiliar code.

---

## 05 - Code Review

File:

```text
05-code-review.md
```

Purpose:

Perform a professional code review and identify issues before creating a pull request.

Output:

- Code quality findings
- Logic issues
- Maintainability concerns
- Performance concerns
- Security concerns
- Best practice recommendations
- Suggested improvements

Recommended Usage:

Before opening a PR or requesting peer review.

---

## 06 - Test and Risk Analysis

File:

```text
06-test-and-risk-analysis.md
```

Purpose:

Validate implementation against requirements and identify missing logic, missing scenarios, edge cases, and potential risks before QA testing.

Output:

- Requirement coverage analysis
- Missing business rules
- Missing validations
- Missing scenarios
- Edge cases
- Potential bugs
- Risk analysis
- Recommended fixes
- QA readiness assessment

Recommended Usage:

After development is completed and before handing over to QA.

Workflow:

```text
Requirement
        ↓
Implementation
        ↓
Test & Risk Analysis
        ↓
Fix Findings
        ↓
QA Testing
```

---

## 07 - Self Review and Fix

File:

```text
07-self-review-and-fix.md
```

Purpose:

Perform a complete self-review cycle and continuously improve the implementation until all identified issues are resolved or no safe fix is possible.

Output:

- Requirement verification
- Scenario generation
- Failure detection
- Root cause analysis
- Safe fix strategy
- Code changes
- Regression verification
- Re-verification loop
- Merge readiness assessment

Recommended Usage:

Before creating a PR or before submitting code for review.

Workflow:

```text
Requirement
        ↓
Implementation
        ↓
Self Review
        ↓
Identify Issues
        ↓
Apply Safe Fixes
        ↓
Re-Review
        ↓
Ready for PR
```

---

# Recommended Development Workflow

For most development tasks:

```text
01 Requirement Analysis
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

For bug fixing:

```text
03 Bug Fix
        ↓
06 Test and Risk Analysis
        ↓
07 Self Review and Fix
        ↓
Create Pull Request
```

For understanding existing code:

```text
04 Code Analysis
        ↓
05 Code Review
        ↓
Implement Changes
```

---

# Notes

These prompts are intentionally technology-independent.

They focus on:

- Software engineering principles
- Business requirements
- Risk reduction
- Maintainability
- Code quality
- Safe implementation practices

The prompts should be adapted to your project's architecture, coding standards, and development workflow.
