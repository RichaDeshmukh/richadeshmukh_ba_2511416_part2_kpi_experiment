# KPI Framework, Business Experiment Analysis & Decision Recommendation

## Repository Information

**Assignment:** Part 2 – KPI Framework, Business Experiment Analysis & Decision Recommendation

**Repository Name:**
`richadeshmukh_ba_2511416_part2_kpi_experiment`

---

# Business Context

A subscription-based digital product company launched a new onboarding and activation campaign to improve user conversion and early engagement.

Users were randomly assigned to one of two groups:

- **Control Group:** Existing onboarding experience
- **Treatment Group:** New onboarding campaign

The objective of this analysis is to determine whether the Treatment experience should be launched to all users based on experimental evidence.

---

# Business Problem

The business must determine whether the new onboarding campaign significantly improves user conversion without negatively impacting customer experience or business performance.

The recommendation should be supported by:

- Experiment analysis
- Statistical hypothesis testing
- KPI evaluation
- Guardrail metric analysis
- Segment-level insights

---

# Dataset Description

The dataset contains user-level information collected during the A/B experiment, including:

- User ID
- Experiment Group (Control/Treatment)
- Landing Page Visit
- Trial Started
- Onboarding Completed
- Paid Conversion
- Revenue
- Refund Requests
- Support Tickets
- Engagement Score
- Days to Convert
- Region
- Device Type
- Traffic Source
- Plan Type

---

# Data Cleaning and Preparation

The dataset was cleaned before analysis by performing the following checks:

- Checked for missing values
- Verified Control and Treatment group counts
- Checked duplicate User IDs
- Validated binary columns (0/1 values)
- Checked revenue for outliers
- Verified segment distribution across experiment groups

No major data quality issues affecting the analysis were identified.

---

# North Star Metric

## Paid Conversion Rate

**Formula**

Paid Conversion Rate = Paid Users / Total Users

### Why this metric?

Paid Conversion Rate directly measures the effectiveness of the onboarding campaign in converting users into paying customers.

Improving this metric contributes directly to:

- Revenue Growth
- Customer Acquisition Efficiency
- Business Profitability

---

# Supporting KPIs

Supporting metrics include:

- Landing Page Visit Rate
- Trial Start Rate
- Onboarding Completion Rate
- Average Revenue Per User
- Average Revenue Per Converted User

---

# KPI Tree Summary

The KPI framework consists of:

## North Star Metric

- Paid Conversion Rate

## Primary Drivers

- Acquisition
- Activation
- Engagement

## Supporting Drivers

- Landing Page Visits
- Trial Starts
- Onboarding Completion
- Revenue
- Customer Experience

## Guardrail Metrics

- Refund Rate
- Support Ticket Rate
- Average Days to Convert
- Engagement Score

---

# Experiment Analysis Approach

The experiment compared the Control and Treatment groups using summary metrics and segment-level analysis.

The following metrics were evaluated:

- User Count
- Landing Page Visit Rate
- Trial Start Rate
- Onboarding Completion Rate
- Paid Conversion Rate
- Average Revenue Per User
- Average Revenue Per Converted User
- Refund Rate
- Support Ticket Rate
- Average Engagement Score
- Average Days to Convert

Segment analysis was performed for:

- Region
- Device Type
- Traffic Source

---

# Hypothesis Test Summary

A one-tailed Two-Sample t-Test (Unequal Variances) was performed to compare the Paid Conversion Rate between the Control and Treatment groups.

### Results

| Metric | Value |
|---------|------:|
| Control Paid Conversion Rate | 3.17% |
| Treatment Paid Conversion Rate | 6.99% |
| p-value | 0.00053 |
| Significance Level | 0.05 |

### Conclusion

Since the p-value is less than 0.05, the Null Hypothesis was rejected.

The Treatment onboarding campaign significantly improved the Paid Conversion Rate compared to the Control group.

---

# Guardrail Metrics Considered

The following guardrail metrics were evaluated:

| Metric | Control | Treatment |
|---------|---------:|----------:|
| Refund Rate | 0.00% | 0.42% |
| Support Ticket Rate | 14.72% | 24.76% |
| Average Engagement Score | 57.05 | 62.90 |
| Average Days to Convert | 8.86 | 6.40 |

### Observation

- Refund Rate remained very low.
- Engagement Score improved.
- Users converted faster.
- Support Ticket Rate increased and should be monitored during rollout.

---

# Final Recommendation

**Recommendation: Launch only for selected segments while monitoring support demand.**

The Treatment group produced a statistically significant improvement in Paid Conversion Rate while increasing user engagement and reducing the average time to convert.

Although the Refund Rate remained low, the increase in Support Ticket Rate indicates that the onboarding experience should be refined before a full rollout.

A phased deployment is recommended, beginning with the highest-performing user segments while continuously monitoring customer support metrics.

---

# Assumptions and Limitations

- The experiment measures short-term campaign performance only.
- Long-term customer retention was not evaluated.
- Customer Lifetime Value (CLV) was outside the scope of this analysis.
- Results may vary across future user populations and business conditions.

---

# Repository Structure

```
part2_kpi_experiment/
├── data/
│   └── campaign_experiment_data.xlsx
├── analysis/
│   ├── experiment_analysis.xlsx
│   └── hypothesis_test_notes.md
├── outputs/
│   ├── kpi_tree.png
│   ├── experiment_summary.xlsx
│   └── recommendation_memo.md
├── screenshots/
│   ├── summary_metrics.png
│   ├── hypothesis_test_output.png
│   └── kpi_tree_preview.png
└── README.md
```

---

# Screenshots Included

The repository includes the following screenshots:

- **summary_metrics.png** – Control vs Treatment summary metrics
- **hypothesis_test_output.png** – Statistical hypothesis test output
- **kpi_tree_preview.png** – KPI Tree visualization

---

# Tools Used

- Microsoft Excel 365
- Excel Pivot Tables
- Excel Data Analysis ToolPak
- GitHub
- Markdown

---

# Conclusion

The experiment demonstrates that the new onboarding campaign significantly improves Paid Conversion Rate and user engagement while reducing the average time to convert.

A phased rollout is recommended to maximize business value while closely monitoring customer support demand and other guardrail metrics.
