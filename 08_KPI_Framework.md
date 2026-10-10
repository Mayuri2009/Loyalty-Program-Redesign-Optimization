# Loyalty Program Redesign & Optimization — KPI Framework

## 1. Purpose

The purpose of this KPI framework is to define measurable indicators for evaluating loyalty program engagement, customer purchasing behavior, reward redemption, and business performance.

The KPIs will help stakeholders establish a baseline, monitor future performance, and evaluate whether proposed loyalty program improvements achieve their intended objectives.

**Note:** This is a simulated portfolio project. The baseline figures below are illustrative and are not verified results from a live business.

---

## 2. Business Objectives

The proposed loyalty program improvements aim to:

- Increase customer participation in the loyalty program.
- Encourage customers to redeem eligible rewards.
- Improve repeat purchasing behavior.
- Monitor spending by loyalty program customers.
- Support data-driven decisions about future loyalty initiatives.

---

## 3. KPI Definitions and Formulas

### KPI 1 — Active Member Rate

**Business question:** What percentage of enrolled customers meet the defined activity criteria?

**Formula:**

Active Member Rate = (Number of Active Members ÷ Total Enrolled Members) × 100

**Baseline:** 3,600 active members out of 10,000 enrolled customers = 36%.

**Definition:** An active member is a customer who meets the agreed activity criteria during the reporting period. For this portfolio analysis, the dataset's existing active-member classification is used; its precise business rule should be confirmed before production use.

**Measurement period:** Monthly, with quarterly trend review.

**Business interpretation:** A low active-member rate may indicate an opportunity to investigate engagement and customer participation.

---

### KPI 2 — Reward Redemption Rate

**Business question:** What percentage of enrolled members have redeemed at least one reward?

**Formula:**

Reward Redemption Rate = (Number of Members Who Redeemed at Least One Reward ÷ Total Enrolled Members) × 100

**Baseline:** 2,100 members who redeemed rewards out of 10,000 enrolled customers = 21%.

**Definition:** A member is counted once if they have completed at least one qualifying reward redemption during the reporting period.

**Measurement period:** Monthly and quarterly.

**Business interpretation:** This KPI helps assess reward usage. It should be interpreted alongside reward eligibility, availability, and redemption rules.

**Important:** The 21% baseline is comparable only if the dataset's 2,100 redeemers and the denominator of 10,000 refer to the same defined reporting period and customer population. Otherwise, recalculate it using consistent period-based data.

---

### KPI 3 — Repeat Purchase Rate

**Business question:** What percentage of qualifying customers made more than one purchase during the reporting period?

**Formula:**

Repeat Purchase Rate = (Number of Qualifying Customers With Two or More Purchases ÷ Total Qualifying Purchasing Customers) × 100

**Baseline reference:** The dataset identifies 4,200 repeat purchasers. The corresponding percentage must be calculated using the defined denominator and matching reporting period.

**Definition:** A repeat purchaser is a qualifying customer with at least two completed purchases during the measurement period.

**Measurement period:** Monthly and quarterly.

**Business interpretation:** A higher repeat purchase rate may indicate stronger purchasing frequency, but it does not by itself prove that the loyalty program caused the behavior.

---

### KPI 4 — Average Spend per Purchasing Member

**Business question:** How much does the average purchasing loyalty member spend during the reporting period?

**Formula:**

Average Spend per Purchasing Member = Total Qualifying Loyalty Member Revenue ÷ Number of Purchasing Loyalty Members

**Baseline reference:** The dataset reports approximately $4.192 million in loyalty-program revenue and an average spend of approximately $420. These figures should be validated against the revenue definition, customer population, and reporting period before they are presented together.

**Definition:** Purchasing members are loyalty members with at least one qualifying purchase during the reporting period.

**Measurement period:** Monthly and quarterly.

**Business interpretation:** This KPI helps monitor spending patterns among purchasing members. It should be reviewed alongside transaction frequency and customer count.

---

### KPI 5 — Loyalty Program Revenue

**Business question:** How much qualifying revenue is associated with loyalty program customers?

**Formula:**

Loyalty Program Revenue = Sum of Qualifying Revenue From Loyalty Member Transactions

**Baseline reference:** Approximately $4.192 million, based on the current portfolio dataset summary.

**Definition:** Revenue must follow a documented business rule for qualifying transactions. Cancelled transactions, returns, refunds, discounts, and duplicate records should be handled consistently.

**Measurement period:** Monthly, quarterly, and annually.

**Business interpretation:** Revenue trends help stakeholders understand the sales contribution associated with loyalty members. This metric alone does not establish incremental revenue caused by the program.

---

## 4. KPI Summary Table

| KPI | Baseline Reference | Reporting Frequency | Business Purpose |
|---|---|---|---|
| Active Member Rate | 36% | Monthly / Quarterly | Monitor member activity |
| Reward Redemption Rate | 21% | Monthly / Quarterly | Monitor reward usage |
| Repeat Purchase Rate | 4,200 repeat purchasers; rate to be validated | Monthly / Quarterly | Monitor repeat purchasing |
| Average Spend per Purchasing Member | Approximately $420; validate definition | Monthly / Quarterly | Monitor spending behavior |
| Loyalty Program Revenue | Approximately $4.192 million; validate scope | Monthly / Quarterly | Monitor revenue associated with loyalty members |

---

## 5. Proposed KPI Targets

The following are examples of **proposed targets for discussion**, not approved business commitments or proven outcomes.

| KPI | Baseline Reference | Illustrative Target | Target Period |
|---|---|---|---|
| Active Member Rate | 36% | 40% | Within 6 months |
| Reward Redemption Rate | 21% | 25% | Within 6 months |
| Repeat Purchase Rate | Establish validated baseline first | Improve by 3 percentage points | Within 6 months |
| Average Spend per Purchasing Member | Validate baseline first | Monitor for improvement against baseline | Within 6 months |
| Loyalty Program Revenue | Validate baseline first | Establish a target after baseline and margin review | Within 6 months |

Targets should be reviewed with business stakeholders before adoption. They should account for seasonality, customer eligibility, campaign costs, profit margins, and the available budget.

---

## 6. Data Quality and KPI Validation

Before publishing KPI results, the Business Analyst or reporting team should verify:

- The reporting period is consistent across numerator and denominator.
- Each customer is counted only once where the KPI requires unique members.
- Active-member and repeat-purchaser definitions are documented.
- Cancelled transactions, returns, and refunds follow agreed revenue rules.
- Duplicate and incomplete records are identified and handled consistently.
- KPI calculations reconcile with the underlying dataset and dashboard.

If the source data does not support a reliable calculation, the KPI should be labelled as requiring validation rather than reported as a confirmed result.

---

## 7. Monitoring and Review Approach

1. Establish and validate the baseline.
2. Confirm KPI definitions and proposed targets with stakeholders.
3. Publish KPI results using consistent calculations.
4. Review trends monthly and investigate material changes.
5. Compare performance with the agreed baseline and targets.
6. Recommend adjustments based on evidence.
7. Evaluate program impact using an appropriate comparison method where possible.

A comparison group or controlled pilot can help distinguish program impact from other factors such as seasonality, promotions, or changes in customer behavior.

---

## 8. Business Analyst's Responsibility

As a Business Analyst, my responsibilities would include:

- Understanding the business objective behind each KPI.
- Defining formulas, denominators, reporting periods, and business rules.
- Validating source data and calculation logic.
- Confirming KPI definitions with relevant stakeholders.
- Documenting assumptions and data limitations.
- Communicating trends and recommending further investigation.
- Supporting the evaluation of whether proposed changes achieve the intended business outcomes.

---

## 9. Conclusion

This KPI framework provides a structured approach to monitoring loyalty member activity, reward redemption, repeat purchasing, spending, and revenue.

The current dataset provides illustrative baseline references. Before using the KPIs for real business decisions, the definitions, reporting periods, calculations, and proposed targets must be validated.

The framework supports evidence-based decision-making without assuming that proposed loyalty program improvements have already produced measurable business results.
