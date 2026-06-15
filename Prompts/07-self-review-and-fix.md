# AI Quality Gate - Self Review and Fix Loop

Analyze the current implementation against the requirement and continuously improve the solution until all identified issues are resolved or no safe fix is possible.

## Input

### Requirement

```text
[paste requirement]
```

### Implementation

```text
[paste code / files / pull request]
```

---

# Objective

Act as a Senior Software Engineer performing a complete pre-merge quality review.

Your responsibilities include:

* Requirement verification
* Business rule validation
* Code analysis
* Test scenario generation
* Failure detection
* Root cause analysis
* Safe bug fixing
* Regression verification
* Merge readiness assessment

The goal is to maximize correctness while preserving existing behavior and minimizing regression risk.

---

## 1. Requirement Verification

Verify that the implementation satisfies:

* Functional requirements
* Business rules
* Validation rules
* Acceptance criteria

Identify:

* Missing requirements
* Incorrect implementations
* Uncovered scenarios
* Ambiguous requirements

---

## 2. Existing Logic Analysis

Analyze the current implementation.

Identify:

* Main execution flow
* Business logic flow
* Validation flow
* Error handling flow
* State transitions
* Dependencies
* Related modules

Explain the current behavior before proposing changes.

---

## 3. Test Scenario Generation

Generate comprehensive scenarios covering:

### Happy Paths

### Validation Rules

### Error Handling

### Edge Cases

### State Transitions

### Permission Scenarios

### Regression Scenarios

For each scenario provide:

* Scenario ID
* Description
* Expected Behavior

---

## 4. Failure Detection

Evaluate the implementation against every generated scenario.

Classify each scenario as:

* PASS
* POTENTIAL FAIL
* UNKNOWN

Provide reasoning.

Do not assume the implementation is correct.

---

## 5. Root Cause Analysis

For every failed or potentially failed scenario identify:

* Root cause
* Impacted logic
* Business impact
* Technical impact
* Regression risk

---

## 6. Safe Fix Strategy

For each identified issue propose the smallest possible fix.

Requirements:

* Preserve existing behavior.
* Preserve business logic.
* Preserve acceptance criteria.
* Preserve component behavior.
* Avoid unnecessary refactoring.
* Avoid architecture changes.
* Avoid modifying unrelated code.
* Minimize regression risk.

Explain why the proposed fix is safe.

---

## 7. Generate Code Changes

Generate only the code changes required to resolve the identified issues.

Do NOT:

* Change business requirements.
* Change acceptance criteria.
* Refactor unrelated code.
* Rename existing structures unnecessarily.
* Modify unrelated functionality.
* Introduce architectural changes.
* Introduce optimization-only changes.

---

## 8. Regression Verification

Verify that:

* Existing functionality remains unchanged.
* Existing business rules remain unchanged.
* Existing validations remain unchanged.
* Existing user flows remain unchanged.

Identify:

* Regression risks
* Affected modules
* Required regression tests

---

## 9. Re-Verification Loop

After generating fixes:

1. Re-evaluate all generated scenarios.
2. Re-check business rules.
3. Re-check validations.
4. Re-check edge cases.
5. Re-check regression risks.

Repeat the analysis until one of the following conditions is met:

* All scenarios are PASS.
* Additional clarification is required.
* A fix would change business requirements.
* A fix would change acceptance criteria.
* A fix would introduce unacceptable regression risk.

---

## 10. Test Execution (Agent Environments Only)

If the environment supports test execution:

Run all related tests.

If any test fails:

1. Analyze the failure.
2. Identify the root cause.
3. Apply the smallest safe fix.
4. Re-run the tests.

Repeat until:

* All tests pass.

OR

* A fix would change business requirements.

OR

* A fix would change acceptance criteria.

OR

* A fix would introduce unacceptable regression risk.

Requirements:

* Do not change business logic.
* Do not modify acceptance criteria.
* Do not refactor unrelated code.
* Do not change component behavior.

---

## 11. Success Criteria

A solution is considered complete only when:

* Requirement coverage is confirmed.
* No known failing scenarios remain.
* No critical regression risks remain.
* Existing behavior is preserved.
* Acceptance criteria remain unchanged.

---

## 12. Stop Conditions

Stop immediately if:

* Requirements are ambiguous.
* Multiple valid business interpretations exist.
* A fix would modify business requirements.
* A fix would modify acceptance criteria.
* A safe fix cannot be determined.
* Additional stakeholder clarification is required.

---

## 13. Final Assessment

Provide:

### Requirement Coverage

### Fixed Issues

### Remaining Risks

### Remaining Unknowns

### Recommended Manual Tests

### Recommended Regression Tests

### Merge Readiness

Choose one:

* Ready to Merge
* Ready with Minor Concerns
* Requires Additional Changes
* Requires Requirement Clarification

Explain the reasoning.
