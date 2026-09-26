# User Stories & Acceptance Criteria
## Loyalty Program Redesign

## US-001 — View Points Balance

### User Story

As a loyalty member, I want to view my current points
balance so that I know how many points I have available.

### Related Requirement

FR-002

### Acceptance Criteria

Given the customer is an active loyalty member

When the customer opens the loyalty account

Then the current points balance should be displayed.

---

## US-002 — View Available Rewards

### User Story

As a loyalty member, I want to see available rewards and
their required points so that I can choose a reward that
I can afford.

### Related Requirement

FR-003

### Acceptance Criteria

Given the customer has a loyalty account

When the customer opens the rewards section

Then available rewards should be displayed

And the points required for each reward should be shown.

---

## US-003 — Redeem Reward

### User Story

As a loyalty member, I want to redeem an eligible reward
so that I can use my accumulated points.

### Related Requirement

FR-004

### Acceptance Criteria

Given the customer has enough points

When the customer selects an eligible reward

Then the system should confirm the redemption

And the required points should be deducted.

---

## US-004 — Apply Reward at Checkout

### User Story

As a customer, I want my selected reward to be applied
during checkout so that I can receive the benefit without
a complicated process.

### Related Requirement

FR-005

### Acceptance Criteria

Given the customer has successfully redeemed a reward

When the customer completes an eligible purchase

Then the reward should be applied to the transaction

And the customer should receive the applicable benefit.

---

## US-005 — Monitor Loyalty KPIs

### User Story

As a business manager, I want to view loyalty program KPIs
so that I can evaluate customer engagement and program
performance.

### Related Requirement

FR-007

### Acceptance Criteria

Given the business manager has access to the loyalty dashboard

When the manager opens the dashboard

Then loyalty KPIs should be displayed

Including active member rate, redemption rate and repeat
purchase rate.

---

## Requirements Traceability

Business Requirement
        ↓
Functional Requirement
        ↓
User Story
        ↓
Acceptance Criteria
        ↓
Test Case
