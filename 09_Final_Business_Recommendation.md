# Loyalty Program Redesign & Optimization — Final Business Recommendations

## 1. Objective

Recommend practical improvements to customer engagement, reward redemption, and loyalty program performance based on the available case-study data and documented testing scenarios.

This is a simulated portfolio project. The recommendations are proposed actions and have not been implemented or validated in a live business environment.

## 2. Key Findings

| Finding | Business Interpretation |
|---|---|
| 10,000 customers are included in the dataset | Provides the customer population for baseline analysis |
| 3,600 customers are classified as active | The active member rate is 36%, subject to the dataset's active-status definition |
| 6,400 customers are classified as inactive | Further analysis is needed to understand inactivity patterns |
| 2,100 customers are recorded as reward redeemers | Redemption behavior should be evaluated against a clearly defined reporting period and eligible-member denominator |
| UAT-002 identified an incorrect points deduction | Redemption calculations require correction and successful retesting before acceptance |

These findings describe the available data and documented test results. They do not, by themselves, establish the causes of customer inactivity or low engagement.

## 3. Prioritized Recommendations

### Priority 1 — Validate and Correct Redemption Rules

**Recommendation:** Review the points calculation and deduction rules for reward redemption.

**Business reason:** UAT-002 failed because the observed points deduction did not match the expected deduction.

**Proposed actions:**
- Confirm the approved points-to-reward conversion rules.
- Validate the calculation before and after redemption.
- Retest successful redemption and insufficient-points scenarios.
- Verify that transaction history and the displayed points balance remain consistent.

**Success measure:** All critical redemption test cases pass, with no unresolved high-severity redemption defects.

### Priority 2 — Simplify the Redemption Journey

**Recommendation:** Assess whether customers can easily understand reward eligibility, required points, and redemption steps.

**Proposed actions:**
- Review the existing redemption steps and eligibility rules.
- Identify confusing or unnecessary steps.
- Test a simplified redemption flow with representative users in a future validation phase.

**Success measures:** Successful redemption rate, redemption abandonment rate, and customer feedback. Establish verified baselines before setting final targets.

### Priority 3 — Investigate Customer Inactivity

**Recommendation:** Analyze inactive customers before deciding which engagement campaigns to introduce.

**Proposed actions:**
- Segment customers by purchase recency and frequency, where the data supports it.
- Review historical engagement and redemption activity.
- Validate possible reasons for inactivity through appropriate customer research.
- Consider targeted re-engagement campaigns only after the findings are reviewed.

**Success measures:** Active member rate, repeat-purchase rate, and campaign engagement rate, using consistent definitions and reporting periods.

### Priority 4 — Establish KPI Monitoring

**Recommendation:** Create a recurring process to monitor loyalty program performance.

**Proposed KPIs:**
- Active member rate
- Reward redemption rate
- Repeat-purchase rate
- Loyalty-attributed revenue, if attribution data is available
- Redemption failure rate
- Points-related defects

**Proposed approach:**
1. Confirm each KPI's definition, denominator, and reporting period.
2. Validate baseline calculations.
3. Agree on realistic targets with business stakeholders.
4. Review performance monthly.
5. Investigate material deviations and document follow-up actions.

Any targets in the KPI framework should remain illustrative until approved by the relevant stakeholders.

## 4. Recommended Implementation Sequence

| Phase | Activity | Expected Deliverable |
|---|---|---|
| 1 | Confirm loyalty business rules | Approved rules and acceptance criteria |
| 2 | Correct and retest redemption behavior | Passed UAT cases and resolved critical defects |
| 3 | Review the redemption journey and inactivity patterns | Validated improvement opportunities |
| 4 | Pilot selected improvements | Pilot results and customer feedback |
| 5 | Monitor KPIs and evaluate results | Performance review and next-step recommendations |

## 5. Risks and Considerations

- Incorrect points calculations may reduce customer trust.
- Unclear KPI definitions may produce misleading conclusions.
- Customer inactivity may have multiple causes that require further validation.
- Proposed changes should be tested before wider implementation.
- Business rules for cancellations, refunds, duplicate requests, and points adjustments must be confirmed before final acceptance.

## 6. Conclusion

The analysis identifies opportunities to improve loyalty program monitoring, investigate customer inactivity, and strengthen the reward redemption process. The failed redemption test also highlights the need to resolve and retest the points deduction issue before UAT acceptance.

The recommended next step is to validate the business rules, resolve the open defect, complete the remaining UAT scenarios, and establish reliable KPI baselines.

**Project status:** Analysis and recommendations documented; implementation and business impact not yet validated.
