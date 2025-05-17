# Hypothesis Tests for Strategic Business Insights


---

## Description

---

This repository contains 10 comprehensive projects focused on applying various statistical hypothesis tests to generate strategic business insights. Each project uses synthetic or real datasets to demonstrate how hypothesis testing can aid in making informed business decisions by validating assumptions, comparing groups, and identifying relationships between variables. The projects span parametric and non-parametric tests to handle different data characteristics and assumptions, providing a robust toolkit for data-driven analysis.

## Table of Contents
- [Description](#description)
- [Projects Overview](#projects-overview)
- [Detailed Project Information](#detailed-project-information)
  - [1. A/B Testing](#1-ab-testing)
  - [2. Chi-Square Test](#2-chi-square-test)
  - [3. Two-Sample T-Test](#3-two-sample-t-test)
  - [4. Paired T-Test](#4-paired-t-test)
  - [5. ANOVA](#5-anova)
  - [6. Correlation Coefficient](#6-correlation-coefficient)
  - [7. Mann-Whitney U Test](#7-mann-whitney-u-test)
  - [8. Wilcoxon Signed-Rank Test](#8-wilcoxon-signed-rank-test)
  - [9. Kruskal-Wallis Test](#9-kruskal-wallis-test)
  - [10. Chi-Square Goodness of Fit Test](#10-chi-square-goodness-of-fit-test)
- [Conclusion](#conclusion)
- [How to Run These Projects](#how-to-run-these-projects)


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

## 1. A/B Testing
📄 Code Link: **[A_B_Testing_Project.ipynb](Hypothesis%20Testing/AB%20Testing/A_B_Testing_Project.ipynb)**

## A/B Testing Project: Evaluating Button Color Impact on User Conversions  

### 📌 Overview  
This project conducts a rigorous A/B testing analysis to evaluate the impact of two different button color variants (Blue vs. Green) on user conversion rates for an e-commerce platform. Using a real-world dataset from Kaggle, the study follows a structured approach, including:  
- **Exploratory Data Analysis (EDA)**  
- **Assumption Verification** (Normality & Homogeneity of Variances)  
- **Statistical Testing** (Independent Samples t-test & Mann-Whitney U Test)  
- **Effect Size & Power Analysis**  
- **Result Interpretation & Business Recommendations**  

🔗 **Dataset Source**: [A/B Testing for Button Color Variants Dataset (Kaggle)](https://www.kaggle.com/datasets/example/ab-testing-button-color)  


### ❓ Problem Statement  
E-commerce platforms continuously experiment with UI elements (like button colors) to maximize user engagement and conversions. However, without proper statistical validation, design changes may not yield meaningful improvements.  

**Key Question**:  
*Does changing the button color (from Blue to Green) lead to a statistically significant increase in user conversion rates?*  


### 🎯 Objective  
- **Determine** if there is a statistically significant difference in conversion rates between the two button colors.  
- **Assess** the practical significance of the change using effect size and power analysis.  
- **Provide** data-driven recommendations for UI optimization.  


### 📊 Dataset Description  
The dataset contains synthetic user interaction data simulating an A/B test with two button variants:  
- **Control Group (A)**: Blue button  
- **Treatment Group (B)**: Green button  

**Key Features**:  
- `user_id`: Unique identifier for each user  
- `group`: Indicates whether the user was in Group A (Control) or Group B (Treatment)  
- `clicked`: Binary indicator (1 = clicked, 0 = did not click)  
- `converted`: Binary indicator (1 = converted, 0 = did not convert)  

**Size**: <1MB (Ideal for quick analysis)  


### 🚀 Project Highlights  
✅ **Comprehensive EDA**: Visualized conversion rates, checked distributions (histograms, Q-Q plots), and compared engagement metrics.  
✅ **Assumption Checks**: Verified normality (Shapiro-Wilk) and homogeneity of variances (Levene’s test).  
✅ **Statistical Testing**:  
   - **Independent Samples t-test** (for normally distributed data)  
   - **Mann-Whitney U Test** (non-parametric alternative)  
✅ **Effect Size & Power Analysis**: Calculated Cohen’s d (effect size) and statistical power to assess practical significance.  
✅ **Actionable Insights**: Provided clear recommendations based on statistical evidence.  


### 🔍 Why This Project?  
- Demonstrates **real-world A/B testing methodology** from hypothesis formulation to result interpretation.  
- Highlights **importance of statistical validation** before implementing UI changes.  
- Provides a **template for data-driven decision-making** in marketing & UX optimization.  


### 💡 Benefits / Use Cases  
📌 **For Businesses**:  
- Helps optimize UI elements to **increase conversions & revenue**.  
- Reduces guesswork by relying on **statistically validated insights**.  

📌 **For Data Scientists**:  
- Serves as a **reference for A/B testing best practices**.  
- Demonstrates **assumption checks, test selection, and interpretation**.  

📌 **For Product Teams**:  
- Guides **data-backed design decisions** for better user engagement.  


### 📈 Statistical Tests Used  
1. **Normality Check**: Shapiro-Wilk Test  
2. **Equal Variance Check**: Levene’s Test  
3. **Hypothesis Testing**:  
   - **Independent Samples t-test** (Parametric)  
   - **Mann-Whitney U Test** (Non-parametric)  
4. **Effect Size**: Cohen’s d  
5. **Power Analysis**: Statistical Power (1 - β)  

### 🔑 Key Findings & Result Summary  
### Hypothesis Testing Results  
- **p-value (t-test)**: **0.927** (Fail to reject H₀)  
- **p-value (Mann-Whitney U)**: **0.928** (Fail to reject H₀)  
- **Conclusion**: **No statistically significant difference** in conversion rates between Blue & Green buttons.  

### Effect Size & Power  
- **Cohen’s d**: **0.500** (Medium effect size)  
- **Statistical Power**: **0.85** (Adequate to detect an effect)  

### Final Recommendation  
📢 **"No significant improvement in conversions was observed when changing the button color from Blue to Green. Thus, retaining the original Blue button is recommended unless further tests with different variations suggest otherwise."**


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

## How to Run These Projects

1. Open the project in [Google Colab](https://colab.research.google.com/)
2. Upload your Excel dataset when prompted.
3. Run all cells in order:
   - Data loading
   - EDA
   - Contingency table creation
   - Visualization
   - Statistical testing
4. Review the final statistical output and visualizations.

---

## Conclusion

This collection of projects provides a foundational understanding of diverse hypothesis testing methods applicable in business contexts. By rigorously checking assumptions and applying appropriate parametric or non-parametric tests, these projects showcase how statistical testing can validate business hypotheses, support decision-making, and uncover actionable insights.

---

