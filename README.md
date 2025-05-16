# Hypothesis Tests for Strategic Business Insights

## Description

This repository contains 10 comprehensive projects focused on applying various statistical hypothesis tests to generate strategic business insights. Each project uses synthetic or real datasets to demonstrate how hypothesis testing can aid in making informed business decisions by validating assumptions, comparing groups, and identifying relationships between variables. The projects span parametric and non-parametric tests to handle different data characteristics and assumptions, providing a robust toolkit for data-driven analysis.

---

## Projects Overview

| Project No. | Project Title                                               |
|-------------|-------------------------------------------------------------|
| 1           | A/B Testing                                                 |
| 2           | Chi-Square Test                                            |
| 3           | Two-Sample T-Test                                          |
| 4           | Paired T-Test                                              |
| 5           | ANOVA                                                      |
| 6           | Correlation Coefficient                                    |
| 7           | Mann-Whitney U Test (Non-parametric alternative to Two-Sample t-test) |
| 8           | Wilcoxon Signed-Rank Test (Non-parametric paired test)    |
| 9           | Kruskal-Wallis Test (Non-parametric ANOVA)                |
| 10          | Chi-Square Goodness of Fit Test                            |

---

## Detailed Project Information

### 1. A/B Testing

**Overview:**  
A/B Testing compares two groups to determine if a new feature or change influences a key business metric.

**Problem Statement:**  
Does a new webpage design increase customer conversion compared to the old design?

**Objective:**  
Test whether the conversion rate differs between control and treatment groups.

**Dataset Description:**  
Synthetic dataset simulating conversion data for two groups.

**Project Highlights:**  
- Hypothesis formulation  
- Normality and homogeneity checks  
- Parametric (t-test) or non-parametric alternatives  
- Power and effect size analysis

**Why This Project?**  
A/B testing is essential for iterative product improvement.

**Benefits / Use Cases:**  
Optimizing marketing campaigns, UX design, product features.

**Statistical Test Used:**  
Independent t-test (or Mann-Whitney U if assumptions violated)

**Key Findings & Result Summary:**  
Significant difference in conversion rates was observed, indicating the new design’s effectiveness.

---

### 2. Chi-Square Test

**Overview:**  
Tests independence between two categorical variables.

**Problem Statement:**  
Is customer satisfaction independent of the service channel?

**Objective:**  
Analyze if satisfaction distribution differs by channel.

**Dataset Description:**  
Categorical synthetic data of customer satisfaction by channel.

**Project Highlights:**  
- Hypotheses on independence  
- Contingency table analysis  
- Chi-square test statistic calculation

**Why This Project?**  
Understanding relationships between categorical variables aids targeted strategies.

**Benefits / Use Cases:**  
Customer feedback analysis, market segmentation.

**Statistical Test Used:**  
Chi-Square Test of Independence

**Key Findings & Result Summary:**  
No significant dependence between satisfaction and channel was found.

---

### 3. Two-Sample T-Test

**Overview:**  
Compares means of two independent groups.

**Problem Statement:**  
Does average sales differ between two regions?

**Objective:**  
Test for mean difference in sales volumes.

**Dataset Description:**  
Synthetic sales data from two regions.

**Project Highlights:**  
- Normality and variance homogeneity checks  
- Parametric two-sample t-test or non-parametric alternative

**Why This Project?**  
Identify regional sales performance differences.

**Benefits / Use Cases:**  
Resource allocation, regional marketing.

**Statistical Test Used:**  
Two-Sample T-Test

**Key Findings & Result Summary:**  
Significant sales difference was observed between regions.

---

### 4. Paired T-Test

**Overview:**  
Compares means of two related groups.

**Problem Statement:**  
Is there a sales increase after a marketing campaign?

**Objective:**  
Analyze sales before and after campaign for same customers.

**Dataset Description:**  
Synthetic paired sales data (before vs after campaign).

**Project Highlights:**  
- Paired data analysis  
- Normality checks on difference scores

**Why This Project?**  
Evaluate effectiveness of interventions.

**Benefits / Use Cases:**  
Campaign effectiveness, process improvements.

**Statistical Test Used:**  
Paired T-Test

**Key Findings & Result Summary:**  
Significant sales increase post-campaign.

---

### 5. ANOVA

**Overview:**  
Tests for mean differences across three or more groups.

**Problem Statement:**  
Do revenues differ by marketing channel?

**Objective:**  
Compare mean revenue among Email, Social Media, and TV campaigns.

**Dataset Description:**  
Synthetic dataset with revenue per campaign type.

**Project Highlights:**  
- Normality and homogeneity checks  
- One-way ANOVA analysis

**Why This Project?**  
Identify most effective marketing channel.

**Benefits / Use Cases:**  
Budget optimization, channel strategy.

**Statistical Test Used:**  
ANOVA (Analysis of Variance)

**Key Findings & Result Summary:**  
No significant difference in mean revenue among channels.

---

### 6. Correlation Coefficient

**Overview:**  
Measures strength and direction of linear relationship between two variables.

**Problem Statement:**  
Is ad spend correlated with revenue?

**Objective:**  
Quantify correlation between advertising costs and sales revenue.

**Dataset Description:**  
Synthetic ad spend and revenue data.

**Project Highlights:**  
- Scatter plot visualization  
- Pearson correlation and significance test

**Why This Project?**  
Understand ROI on advertising.

**Benefits / Use Cases:**  
Budget planning, forecasting.

**Statistical Test Used:**  
Pearson Correlation Coefficient

**Key Findings & Result Summary:**  
Weak, non-significant correlation found between ad spend and revenue.

---

### 7. Mann-Whitney U Test

**Overview:**  
Non-parametric alternative to two-sample t-test for independent groups.

**Problem Statement:**  
Are sales distributions different between two regions where normality is violated?

**Objective:**  
Test for differences without assuming normality.

**Dataset Description:**  
Synthetic sales data violating normality.

**Project Highlights:**  
- Data visualization to check distribution  
- Mann-Whitney U test applied

**Why This Project?**  
Robust testing under non-normal data.

**Benefits / Use Cases:**  
Non-parametric testing when assumptions fail.

**Statistical Test Used:**  
Mann-Whitney U Test

**Key Findings & Result Summary:**  
No significant difference in sales distributions between regions.

---

### 8. Wilcoxon Signed-Rank Test

**Overview:**  
Non-parametric alternative to paired t-test.

**Problem Statement:**  
Is there a difference in customer satisfaction before and after a service change, without assuming normality?

**Objective:**  
Analyze paired differences non-parametrically.

**Dataset Description:**  
Synthetic paired satisfaction scores.

**Project Highlights:**  
- Check data for normality violations  
- Wilcoxon Signed-Rank test application

**Why This Project?**  
Paired comparisons with non-normal data.

**Benefits / Use Cases:**  
Customer satisfaction studies, repeated measures.

**Statistical Test Used:**  
Wilcoxon Signed-Rank Test

**Key Findings & Result Summary:**  
Significant difference found in satisfaction scores pre- and post-service change.

---

### 9. Kruskal-Wallis Test

**Overview:**  
Non-parametric alternative to ANOVA.

**Problem Statement:**  
Do sales differ across marketing channels when data normality is violated?

**Objective:**  
Test for differences among three or more independent groups.

**Dataset Description:**  
Synthetic non-normal sales data for multiple campaigns.

**Project Highlights:**  
- Visualization and assumption checks  
- Kruskal-Wallis test application

**Why This Project?**  
Robust multi-group comparison without normality assumption.

**Benefits / Use Cases:**  
Marketing analysis, product performance.

**Statistical Test Used:**  
Kruskal-Wallis Test

**Key Findings & Result Summary:**  
No significant sales differences across channels.

---

### 10. Chi-Square Goodness of Fit Test

**Overview:**  
Tests if observed frequencies match expected frequencies.

**Problem Statement:**  
Does customer distribution across campaigns differ from expected proportions?

**Objective:**  
Evaluate fit between observed and expected counts.

**Dataset Description:**  
Synthetic frequency counts of customers by campaign.

**Project Highlights:**  
- Frequency table creation  
- Chi-square goodness of fit test

**Why This Project?**  
Check if observed behavior matches business expectations.

**Benefits / Use Cases:**  
Resource allocation, campaign targeting.

**Statistical Test Used:**  
Chi-Square Goodness of Fit Test

**Key Findings & Result Summary:**  
Observed distribution aligns with expected customer distribution.

---

## Conclusion

This collection of projects provides a foundational understanding of diverse hypothesis testing methods applicable in business contexts. By rigorously checking assumptions and applying appropriate parametric or non-parametric tests, these projects showcase how statistical testing can validate business hypotheses, support decision-making, and uncover actionable insights.

---

## How to Run These Projects

1. Clone this repository:  
   ```bash
   git clone <repository-url>
   cd <repository-folder>
