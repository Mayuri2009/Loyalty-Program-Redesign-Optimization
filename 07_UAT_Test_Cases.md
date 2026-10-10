# Loyalty Program Redesign & Optimization — UAT Test Cases

## 1. Purpose

The purpose of User Acceptance Testing (UAT) is to verify whether the proposed loyalty program solution meets the defined business requirements and works as expected from the customer's perspective.

This document defines test scenarios, expected results, actual results, test status, and defect tracking.

**Note:** This is a simulated portfolio project. The test scenarios and results are illustrative and do not represent testing of a live production system.

---

## 2. UAT Scope

The UAT covers the following business functions:

- Viewing loyalty points balance
- Redeeming loyalty points
- Validating reward eligibility
- Preventing incorrect point deductions
- Reviewing loyalty program information

---

## 3. UAT Test Cases

| Test Case ID | Test Scenario | Expected Result | Illustrative Actual Result | Status |
|---|---|---|---|---|
| UAT-001 | View loyalty points balance | The customer sees the correct available points balance. | The displayed balance matches the recorded balance. | PASS |
| UAT-002 | Redeem eligible loyalty points | The correct number of points is deducted after successful redemption. | An incorrect number of points is deducted in the illustrative scenario. | FAIL |
| UAT-003 | Attempt redemption with insufficient points | The system prevents redemption and displays an appropriate message. | Redemption is blocked when the balance is insufficient. | PASS |
| UAT-004 | Attempt to redeem an expired or unavailable reward | The system prevents redemption of an ineligible reward. | The ineligible reward cannot be redeemed. | PASS |
| UAT-005 | Review loyalty transaction history | The customer can view the relevant loyalty transaction details. | The transaction history displays the recorded details. | PASS |

**Status definitions:**

- **PASS:** The observed result meets the expected result.
- **FAIL:** The observed result does not meet the expected result.
- **BLOCKED:** Testing cannot proceed because of a dependency or unresolved issue.
- **NOT RUN:** The test has not yet been executed.

---
## 3.1 Additional Negative and Boundary Test Cases

The following test cases extend the existing UAT coverage by checking exceptional conditions and transaction accuracy.

**Note:** These are proposed test scenarios. They should be marked as NOT RUN until actually executed in an appropriate test environment.

| Test Case ID | Test Scenario | Expected Result | Actual Result | Status |
|---|---|---|---|---|
| UAT-006 | Attempt redemption when the customer has exactly the minimum required points. | Redemption succeeds if the customer meets all eligibility rules, and the correct points are deducted. | Not executed. | NOT RUN |
| UAT-007 | Attempt redemption when the customer has fewer points than required. | Redemption is rejected, the points balance remains unchanged, and an appropriate message is displayed. | Not executed. | NOT RUN |
| UAT-008 | Submit the same redemption request twice. | The system prevents duplicate processing and deducts points only once. | Not executed. | NOT RUN |
| UAT-009 | Process a refund or cancellation for an eligible purchase. | Points are adjusted according to the documented loyalty business rules, and the transaction history remains accurate. | Not executed. | NOT RUN |

### Additional Validation Notes

- UAT-006 validates behavior at the minimum eligibility boundary.
- UAT-007 validates rejection when the points balance is insufficient.
- UAT-008 validates duplicate-redemption protection.
- UAT-009 validates consistency between refunds, cancellations, and loyalty-point adjustments.

Before execution, the relevant business rules must be confirmed, particularly for refund-related point adjustments.

Any failed test should be recorded in the defect log, linked to the relevant requirement, corrected, and retested.

These additional cases demonstrate proposed test coverage and must not be presented as successfully executed tests without supporting evidence.  

## 4. Defect Log

| Defect ID | Related Test Case | Defect Description | Severity | Status |
|---|---|---|---|---|
| DEF-001 | UAT-002 | The system deducts an incorrect number of loyalty points during redemption. | High | Open |

### Defect Details

**Expected behavior:** The system should deduct only the eligible number of points required for the selected redemption.

**Observed behavior:** The illustrative test scenario records an incorrect points deduction.

**Business impact:** Incorrect deductions can reduce customer trust, create complaints, and lead to loyalty balance disputes.

**Required corrective action:**

1. Investigate the points calculation and redemption rules.
2. Correct the calculation or business logic.
3. Retest the affected redemption scenario.
4. Verify that the updated points balance is accurate.
5. Record the retest result and close the defect only after successful verification.

---

## 5. UAT Entry and Exit Criteria

### Entry Criteria

- Business requirements and acceptance criteria are documented.
- Test scenarios are prepared and reviewed.
- Test data and the required test environment are available.
- Expected results are defined for each test case.

### Exit Criteria

- All required test cases have been executed.
- Failed test cases have been investigated.
- High-severity defects have been resolved and successfully retested.
- Test evidence and defect status are documented.
- The appropriate business representative reviews the results and records the acceptance decision.

---

## 6. Overall UAT Status

**Current illustrative status: Pending Final Acceptance**

UAT cannot be considered fully accepted while DEF-001 remains open and UAT-002 is failing.

Final acceptance should be recorded only after the defect is resolved, the affected test case passes retesting, and the exit criteria are satisfied.

No production implementation or actual business acceptance is claimed in this portfolio project.

---

## 7. UAT Execution and Sign-Off Process

1. Execute the test cases against the documented requirements.
2. Compare actual results with expected results.
3. Record PASS, FAIL, BLOCKED, or NOT RUN.
4. Log defects for failed test cases.
5. Assign corrective actions and resolve defects.
6. Retest the affected scenarios and document evidence.
7. Review the final results against the exit criteria.
8. Obtain the appropriate business acceptance decision.

### UAT Flow

Requirements → Test Case Preparation → Test Execution → Result Validation → Defect Logging → Correction and Retesting → Final Acceptance Decision

---

## 8. Business Analyst's Responsibility

As a Business Analyst, my responsibilities in the UAT process would include:

- Ensuring test scenarios trace back to business requirements.
- Confirming that expected results reflect agreed business rules.
- Helping clarify defects and their business impact.
- Coordinating with relevant business and technical stakeholders.
- Maintaining traceability between requirements, test cases, and defects.
- Supporting retesting and documenting the final acceptance decision.

---

## 9. Conclusion

UAT helps confirm that a proposed loyalty program solution meets business requirements and supports the intended customer experience.

In this illustrative scenario, the incorrect points deduction must be corrected and retested before final acceptance. This demonstrates the importance of defect tracking, requirement validation, and business approval in the Business Analysis lifecycle.
