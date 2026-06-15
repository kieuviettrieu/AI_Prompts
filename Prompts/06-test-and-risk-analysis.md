# Pre-QA Validation and Gap Analysis Prompt

Analyze the requirement and implementation before QA handoff.

Your goal is to identify:

- Missing requirements
- Missing business rules
- Missing validations
- Missing scenarios
- Potential bugs
- Edge cases
- Regression risks
- Incomplete implementations

Focus on actionable findings that help a Software Engineer quickly identify and resolve gaps before QA testing.

---

## Input

### Requirement

[paste requirement]

### Implementation

[paste code / files / pull request]

---

## Step 1: Requirement Analysis

Analyze and identify:

- Feature purpose
- Business objective
- Expected behavior
- Explicit business rules
- Implicit business rules
- Validation requirements
- State transition requirements
- Permission requirements

Highlight:

- Missing requirements
- Ambiguous requirements
- Assumptions made by the implementation

---

## Step 2: Scenario Analysis

Identify all relevant scenarios.

Include:

### Happy Paths

### Alternate Flows

### Validation Scenarios

### Error Handling Scenarios

### State Transition Scenarios

### Permission Scenarios

### Regression Scenarios

### Edge Cases

Examples:

- Invalid inputs
- Missing data
- Duplicate actions
- Concurrent actions
- Unexpected user behavior
- Large data volumes
- State conflicts

---

## Step 3: Requirement Coverage Verification

Compare the implementation against every identified requirement and business rule.

For each requirement determine:

- Covered
- Partially Covered
- Missing
- Incorrect
- Unknown

Use actual code evidence whenever possible.

Do not assume the implementation is correct.

---

## Step 4: Gap Analysis

Identify every gap between:

- Requirement vs Implementation
- Business Rule vs Implementation
- Expected Behavior vs Actual Behavior

For every gap determine:

- What is missing
- Why it is missing
- Where it is missing
- Why it matters
- How it should be fixed

---

## Step 5: Risk Analysis

Identify:

### Functional Risks

### Business Risks

### Technical Risks

### Regression Risks

Consider:

- Existing user flows
- Existing business rules
- Existing validations
- Related modules
- Shared components
- Shared services

---

## Step 6: Developer-Focused Findings Report

Generate findings ONLY for items that are:

- Missing
- Partially Covered
- Incorrect
- High Risk

For each finding provide:

### Finding ID

### Severity

Choose one:

- Critical
- High
- Medium
- Low

### Location

Identify:

- File
- Component
- Service
- API
- Method
- Function

If exact location is unknown:

- State the most likely location.

### Issue

Clearly explain:

- What is missing
- What is incorrect
- What scenario is not handled

### Root Cause

Explain why the issue exists.

### Impact

Explain:

- Functional impact
- Business impact
- User impact

### Recommended Fix

Provide the smallest safe change required.

Requirements:

- Preserve existing behavior.
- Preserve business rules.
- Preserve acceptance criteria.
- Avoid unnecessary refactoring.
- Avoid architecture changes.
- Avoid modifying unrelated code.
- Minimize regression risk.

Do NOT generate full code unless explicitly requested.

---

## Step 7: Final Summary

Provide:

### Requirement Coverage

Example:

85%

### Findings Summary

Example:

- Critical: X
- High: X
- Medium: X
- Low: X

### Blocking Issues

List all Critical and High findings.

### Regression Risk

Choose:

- Low
- Medium
- High

### Ready For QA

Choose:

- Yes
- No

### Next Action

Provide the recommended next step before QA handoff.

---

## Output Format

Use the following format:

# Findings

## F-001 - [Short Title]

Severity: Critical | High | Medium | Low

Location:

- File:
- Component:
- Service:
- Method:

Issue:

- What is missing or incorrect.

Root Cause:

- Why the issue exists.

Impact:

- Functional impact
- Business impact
- User impact

Recommended Fix:

- Smallest safe change required.

---

# Summary

Requirement Coverage: XX%

Critical Issues: X

High Issues: X

Medium Issues: X

Low Issues: X

Regression Risk: Low | Medium | High

Ready For QA: Yes | No

Blocking Issues:

- F-001
- F-002

Next Action:

- Recommended next step.