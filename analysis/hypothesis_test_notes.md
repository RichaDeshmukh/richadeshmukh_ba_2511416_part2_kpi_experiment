# Hypothesis Test Notes

## Business Objective

The objective is to determine whether the new onboarding campaign (Treatment) significantly improves the Paid Conversion Rate compared to the existing onboarding experience (Control).

---

## Metric Being Tested

**Paid Conversion Rate**

Formula:

Paid Conversion Rate = Number of Paid Users / Total Users

---

## Null Hypothesis (H₀)

There is no statistically significant difference in Paid Conversion Rate between the Control and Treatment groups.

---

## Alternative Hypothesis (H₁)

The Treatment group has a higher Paid Conversion Rate than the Control group.

---

## Type of Test

One-tailed test

Reason:
The business objective is specifically to determine whether the Treatment performs **better** than the Control, not merely whether it is different.

---

## Significance Level

α = 0.05 (95% confidence level)

---

## Decision Rule

If the p-value < 0.05:

Reject the Null Hypothesis.

Otherwise:

Fail to reject the Null Hypothesis.

---

## Business Interpretation

If the Treatment group demonstrates a statistically significant improvement in Paid Conversion Rate without negatively affecting guardrail metrics, the company should consider launching the new onboarding experience.az

---

# Test Results

## Test Inputs

| Item | Value |
|------|------:|
| Test Used | Two-Sample t-Test (Unequal Variances) |
| Primary Metric | Paid Conversion Rate |
| Control Sample Size | 693 users |
| Treatment Sample Size | 715 users |
| Significance Level (α) | 0.05 |

---

## Test Output

| Statistic | Value |
|-----------|------:|
| Control Mean | 0.0317 (3.17%) |
| Treatment Mean | 0.0699 (6.99%) |
| t Statistic | -3.2801 |
| One-tailed p-value | 0.00053 |

---

## Decision

Since the one-tailed p-value (0.00053) is less than the significance level (0.05), the Null Hypothesis is rejected.

---

## Business Interpretation

The statistical test indicates that the Treatment onboarding campaign significantly improved the Paid Conversion Rate compared with the Control group. The observed increase from **3.17%** to **6.99%** is statistically significant and is unlikely to have occurred by random chance.

However, the final business recommendation should also consider guardrail metrics such as Refund Rate, Support Ticket Rate, Average Days to Convert, and Engagement Score before deciding whether to launch the new onboarding experience for all users.