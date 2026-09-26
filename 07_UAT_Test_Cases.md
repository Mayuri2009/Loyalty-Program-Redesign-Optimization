# UAT — Loyalty Program Redesign

## 1. Objective

The objective of UAT is to verify that the proposed loyalty
program functionality meets the defined business requirements
and acceptance criteria.

## 2. UAT Test Cases

| Test ID | Requirement | Test Scenario | Expected Result | Status |
|----------|-------------|---------------|-----------------|--------|
| TC-001 | FR-002 | View points balance | Correct balance displayed | PASS |
| TC-002 | FR-003 | View available rewards | Rewards and required points displayed | PASS |
| TC-003 | FR-004 | Redeem eligible reward | Reward confirmed and points deducted | PASS |
| TC-004 | FR-005 | Apply reward at checkout | Reward correctly applied | PASS |
| TC-005 | FR-007 | Open KPI dashboard | Required KPIs displayed | PASS |

## 3. Detailed UAT Example

### TC-003 — Redeem Eligible Reward

#### Preconditions

- Customer has a valid loyalty account.
- Customer has enough points.
- Reward is available.

#### Test Steps

1. Open loyalty account.
2. View available rewards.
3. Select eligible reward.
4. Click Redeem.
5. Confirm redemption.

#### Expected Result

Reward redemption is confirmed and the required points
are deducted from the customer's balance.

#### Actual Result

Reward successfully redeemed and required points deducted.

#### Status

PASS

## 4. Example Defect

### DEF-001

Issue:
Incorrect points deduction during reward redemption.

Expected:
1,000 points deducted.

Actual:
1,500 points deducted.

Severity:
High

Status:
Open

## 5. UAT Sign-Off

UAT Status: ACCEPTED

The tested functionality meets the defined acceptance
criteria for the current release. No critical outstanding
defects remain.
