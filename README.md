# 🚀 Hypothesis Tests for Strategic Business Insights


---

## 📌 Description

---

This repository contains 10 comprehensive projects focused on applying various statistical hypothesis tests to generate strategic business insights. Each project uses synthetic or real datasets to demonstrate how hypothesis testing can aid in making informed business decisions by validating assumptions, comparing groups, and identifying relationships between variables. The projects span parametric and non-parametric tests to handle different data characteristics and assumptions, providing a robust toolkit for data-driven analysis.

## 📁 Table of Contents
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
- [Technical Implementation](#technical-implementation)
- [How to Run These Projects](#how-to-run-these-projects)
- [Conclusion](#conclusion)



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
📄 **Project Link:** **[A_B_Testing_Project.ipynb](Hypothesis%20Testing/AB%20Testing/A_B_Testing_Project.ipynb)**

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

## 2. Chi-Square Test

## **Chi-Square Test Project: Gender vs Purchase Likelihood Analysis**  

📄 **Project Link:** **[Chi_Square_Testing.ipynb](Hypothesis%20Testing/Chi-Square%20Test/Chi_Square_Testing.ipynb)**

### 📌 Overview  
This project employs the **Chi-Square Test of Independence** to investigate whether a statistically significant association exists between customer gender and product purchase likelihood in an e-commerce context. Using a carefully crafted synthetic dataset that mimics real-world shopping behavior, the analysis includes:  
- Data visualization of key variables (gender, purchase status, age)  
- Contingency table construction  
- Chi-Square test assumption verification  
- Statistical testing and interpretation  
- Actionable business insights  


###  ❓ Problem Statement  
E-commerce businesses often wonder if demographic factors like gender influence purchasing decisions. This analysis answers:  
**"Does customer gender significantly affect the likelihood of purchasing our product?"**  


###  🎯 Objective  
- Determine if gender and purchase likelihood are statistically associated  
- Validate assumptions for Chi-Square testing  
- Provide data-driven recommendations for marketing strategies  


###  📊 Dataset Description  
**Synthetic Dataset** (500 records) simulating real customer behavior:  
- `Gender`: Binary (Male/Female) with near-equal distribution  
- `Purchase`: Binary (Yes/No) with gender-biased probabilities  
- `Age`: Normally distributed (μ=35, σ=10), clipped to 18-70 years  

**Key Characteristics**:  
✅ Balanced gender distribution (Male: 233, Female: 267)  
✅ Realistic purchase probability variation (Male: 45%, Female: 55%)  
✅ Numeric age variable for additional demographic analysis  


###  🚀 Project Highlights  
✅ **Comprehensive EDA**: Countplots, histograms, and contingency tables  
✅ **Assumption Verification**:  
   - Independence of observations  
   - Expected frequencies ≥5 (all cells satisfied)  
✅ **Statistical Testing**:  
   - Chi-Square Test of Independence  
   - Effect size calculation (Cramer's V optional)  
✅ **Clear Interpretation**: Business-focused conclusions  


###  🔍 Why This Project?  
- Demonstrates **real-world application** of Chi-Square testing  
- Highlights **importance of assumption checks** in statistical analysis  
- Provides **template for customer segmentation studies**  


###  💡 Benefits / Use Cases  
📌 **For Marketing Teams**:  
- Avoids gender-based assumptions in campaigns  
- Guides resource allocation for promotions  

📌 **For Data Scientists**:  
- Complete workflow from synthetic data generation to interpretation  
- Best practices for categorical data analysis  

📌 **For Product Managers**:  
- Evidence-based decisions on product positioning  


###  📈 Statistical Tests Used  
1. **Chi-Square Test of Independence**  
   - Test Statistic: χ² = 1.9395  
   - Degrees of Freedom: 1  
   - p-value: 0.1641  
2. **Expected Frequency Verification**  
3. **Effect Size Measurement** (Optional: Cramer's V/Phi Coefficient)  


### **🔑 Key Findings & Result Summary**  
**Hypothesis Testing Results:**  
- **p-value**: 0.1641 (> 0.05 significance level)  
- **Conclusion**: Fail to reject null hypothesis  

**Business Interpretation:** 
📢 **"No statistically significant association found between gender and purchase likelihood. Marketing strategies should not prioritize gender-based targeting for this product."**  

### Supplementary Insights  
- Observed purchase rates:  
  - Female: 55%  
  - Male: 45%  
- While numeric differences exist, they're **not statistically significant**
  
---

## 3. Two-Sample T-Test

## 📊 **Two-Sample T-Test: Revenue Comparison Between North and South Regions**  

📄 **Project Link:** **[Two-Sample T-Test.ipynb](Hypothesis%20Testing/Hypothesis%20Tests/1.%20Two-Sample%20T-Test.ipynb)**

### 🌐 Overview  
This project performs a Two-Sample Independent t-test to analyze whether there's a statistically significant difference in average revenue between North and South regions of a retail business. Using a carefully generated synthetic dataset, we:  
• Visualize revenue distributions  
• Validate statistical assumptions  
• Conduct hypothesis testing  
• Derive business insights  

### ❓ Problem Statement  
A retail chain observes slight revenue differences between its North and South locations. Management needs to know:  
*"Is this observed difference statistically significant, or just random variation?"*  

### 🎯 Objective  
• Determine if regional revenue differences are statistically meaningful  
• Demonstrate proper t-test application with assumption checks  
• Provide data-backed recommendations for regional strategy  

### 📊 Dataset Description  
**Synthetic Revenue Data (500 records):**  
• **North Region (250 samples):**  
  - Mean: $50,000  
  - Standard Deviation: $8,000  
• **South Region (250 samples):**  
  - Mean: $51,000  
  - Standard Deviation: $8,500  

**Variables:**  
• `region`: Categorical (North/South)  
• `revenue`: Continuous numerical values  

### 🚀 Project Highlights  
✅ **Data Visualization:**  
   - Histograms with KDE plots  
   - Q-Q plots for normality inspection  

✅ **Rigorous Assumption Testing:**  
   - Shapiro-Wilk normality test (North p=0.126, South p=0.884)  
   - Levene's test for equal variances  

✅ **Proper Statistical Testing:**  
   - Independent Two-Sample t-test implementation  
   - Correct interpretation of p-values  

✅ **Business-Ready Conclusions:**  
   - Clear statistical findings translated to actionable insights  

### 🔍 Why This Project Matters  
• Real-world demonstration of t-test methodology  
• Emphasizes critical assumption validation step  
• Provides template for regional performance analysis  

### 💡 Business Value  
📌 **For Executives:**  
   - Evidence-based regional strategy decisions  
   - Avoids overreacting to random fluctuations  

📌 **For Analysts:**  
   - Complete t-test workflow example  
   - Proper assumption checking techniques  

📌 **For Store Managers:**  
   - Understands true performance differences  
   - Guides resource allocation decisions  

### 📈 Statistical Tests Performed  
1. **Normality Testing:**  
   - Shapiro-Wilk Test (Both regions p > 0.05 → Normally distributed)  

2. **Equal Variance Testing:**  
   - Levene's Test (p = 0.423 → Equal variances assumed)  

3. **Two-Sample t-test Results:**  
   - t-statistic: -1.593  
   - p-value: 0.112  
   - 95% Confidence Interval: (-2193.5, 228.3)  

### 🔑 Key Findings  
• **p-value = 0.112** (> 0.05 threshold)  
• **Conclusion:** Fail to reject null hypothesis  

### Business Interpretation  

📢**Despite the $1,000 higher average revenue in South region, this difference is **not statistically significant**. Regional strategies should focus on factors beyond geography to improve revenue.**


---

## 4. Paired T-Test

📄 **Project Link:** **[Paired T-Test.ipynb](Hypothesis%20Testing/Hypothesis%20Tests/2.%20Paired%20T-Test.ipynb)**

## **📊 Paired T-Test Analysis: Measuring Ad Campaign Effectiveness** 

### 🌟 Overview  
This project uses a **Paired T-Test** to evaluate whether an advertising campaign significantly impacted product sales across 30 stores. By comparing pre-campaign and post-campaign sales data from the same stores, we:  
• Verified statistical assumptions  
• Calculated meaningful effect sizes  
• Provided actionable business recommendations  

### ❓ Problem Statement  
"Did our recent marketing campaign actually increase store sales, or are the observed improvements just random fluctuations?"  

### 🎯 Objective  
• Quantify the campaign's impact with 95% confidence  
• Demonstrate proper paired test methodology  
• Guide future marketing investment decisions  

### 📊 Dataset Description  
**Synthetic Sales Data (30 Stores):**  
• **Before Campaign:**  
  - Mean Sales: 200 units  
  - Standard Deviation: 20 units  
• **After Campaign:**  
  - Mean Sales: ~210 units (+5% lift)  
  - Added Noise: N(10,15)  

**Key Variables:**  
• `Store_ID`: Unique identifier  
• `Before_Campaign`: Daily avg sales (pre-intervention)  
• `After_Campaign`: Daily avg sales (post-intervention)  

### 🚀 Project Highlights  
✅ **Assumption Validation:**  
   - Shapiro-Wilk test (p=0.913 → normally distributed differences)  
   - Visual checks via Q-Q plots and histograms  

✅ **Robust Analysis:**  
   - Proper handling of paired observations  
   - Correct interpretation of directional change  

✅ **Business-Ready Insights:**  
   - Clear effect size calculation  
   - Statistical significance with practical interpretation  

### 🔍 Why This Matters  
• Real-world example of **within-subjects** analysis  
• Shows why paired tests outperform independent tests for before/after studies  
• Provides template for marketing ROI measurement  

### 💡 Value Proposition  
📌 **For Marketing Teams:**  
   - Proof of campaign effectiveness  
   - Justification for future budgets  

📌 **For Store Managers:**  
   - Quantified performance impact  
   - Benchmark for future initiatives  

📌 **For Data Teams:**  
   - Complete paired test workflow  
   - Assumption checking best practices  

### 📈 Statistical Approach  
1. **Normality Testing:**  
   - Shapiro-Wilk on paired differences (p > 0.05 → normal)  

2. **Paired T-Test Results:**  
   - t-statistic: 3.209  
   - p-value: 0.0032  
   - Mean Difference: +10 units  
   - 95% CI: [3.8, 16.2]  

### 🔑 Key Findings  
• **Highly Significant Result** (p = 0.0032)  
• **Average Lift:** +10 units per store (5% increase)  
• **Confidence:** 95% certain true effect is between +3.8 to +16.2 units  

### Executive Conclusion  
📢 **The advertising campaign **successfully increased sales** by an average of 10 units per store (p < 0.01). This statistically significant result suggests the campaign should be considered for scaling to other markets.**


---

## 5. ANOVA

📄 **Project Link:** **[ANOVA Test](Hypothesis%20Testing/Hypothesis%20Tests/3.%20ANOVA%20Test.ipynb)**

## 📊 **ANOVA Analysis: Comparing Marketing Campaign Effectiveness**  

### 🌟 Overview  
This project employs **One-Way ANOVA** to evaluate whether three marketing campaigns (Email, Social Media, TV) generate significantly different revenue outcomes. Through rigorous assumption checks and statistical testing, we provide data-driven insights for marketing strategy optimization.

### ❓ Problem Statement  
"Do our different marketing campaigns (Email vs. Social Media vs. TV) produce meaningfully different revenue results, or are observed variations just random?"

### 🎯 Objective  
• Determine if campaign type affects revenue generation  
• Validate ANOVA assumptions for reliable results  
• Guide future marketing budget allocation  

### 📊 Dataset Description  
**Synthetic Revenue Data (90 Customers):**  
• **Email Campaign (30):**  
  - Mean: $250  
  - SD: $30  
• **Social Media (30):**  
  - Mean: $270  
  - SD: $25  
• **TV Campaign (30):**  
  - Mean: $260  
  - SD: $35  

**Variables:**  
• `campaign_type`: Categorical (3 levels)  
• `revenue`: Continuous numerical values  

### 🚀 Project Highlights  
✅ **Comprehensive Assumption Checks:**  
   - Normality per group (Shapiro-Wilk all p > 0.05)  
   - Homogeneity of variance (Levene's p = 0.084)  
   - Independence by design  

✅ **Robust Statistical Testing:**  
   - Proper ANOVA implementation  
   - Effect size calculation (η² optional)  

✅ **Actionable Visualization:**  
   - Boxplots showing revenue distributions  
   - Q-Q plots for normality verification  

### 🔍 Why This Matters  
• Demonstrates proper **multi-group comparison** methodology  
• Highlights importance of **assumption validation** before ANOVA  
• Provides framework for **marketing ROI analysis**  

### 💡 Business Value  
📌 **For CMOs:**  
   - Data-backed campaign evaluation  
   - Objective budget allocation guidance  

📌 **For Marketing Teams:**  
   - Identifies equally effective channels  
   - Prevents over-investment in underperforming campaigns  

📌 **For Data Teams:**  
   - Complete ANOVA workflow example  
   - Assumption checking best practices  

### 📈 Statistical Approach  
1. **Assumption Verification:**  
   - Shapiro-Wilk normality tests (All groups p > 0.05)  
   - Levene's test for equal variances (p = 0.084)  

2. **One-Way ANOVA Results:**  
   - F-statistic: 1.699  
   - p-value: 0.189  
   - Group Means:  
     • Email: $250  
     • Social: $270  
     • TV: $260  

### 🔑 Key Findings  
• **High p-value (0.189 > 0.05)** → Fail to reject null  
• **No significant revenue differences** between campaigns  
• Observed $20 variations likely due to random chance  

###  Strategic Conclusion  
📢 **All three campaigns perform **statistically similarly** in revenue generation (p = 0.19). Marketing budgets could be allocated based on other factors like customer reach or cost efficiency rather than expected revenue differences.**

---

## 6. Correlation Coefficient

📄 **Project Link:** **[Correlation_Coefficient.ipynb](Hypothesis%20Testing/Hypothesis%20Tests/4_Correlation_Coefficient.ipynb)**

## 📈 **Correlation Analysis: Advertising Spend vs Revenue** 

### 🌟 Overview  
This project investigates the relationship between advertising expenditure and revenue generation using Pearson's correlation coefficient. Through synthetic data modeling and rigorous statistical testing, we determine whether increased ad spending reliably predicts higher revenue.

### ❓ Problem Statement  
"Does increasing our advertising budget lead to proportionally higher revenue, or are other factors more influential?"  

### 🎯 Objective  
• Quantify the ad spend-revenue relationship  
• Validate statistical assumptions for correlation analysis  
• Provide data-driven marketing investment guidance  

### 📊 Dataset Description  
**Synthetic Marketing Data (100 Weeks):**  
• **Advertising Spend:**  
  - Mean: $10,000  
  - SD: $2,000  
  - Normally distributed  
• **Revenue:**  
  - Weak linear relationship (5% of ad spend)  
  - Added noise: N(500,500)  

**Variables:**  
• `ad_spend`: Continuous numerical (USD)  
• `revenue`: Continuous numerical (USD)  

### 🚀 Project Highlights  
✅ **Comprehensive Assumption Checks:**  
   - Normality confirmed (Shapiro-Wilk p > 0.05)  
   - Variance homogeneity verified  

✅ **Robust Statistical Testing:**  
   - Pearson's r calculation  
   - Two-tailed significance testing  

✅ **Practical Interpretation:**  
   - Business-focused conclusions  
   - Clear effect size reporting  

### 🔍 Why This Matters  
• Demonstrates proper **bivariate correlation** analysis  
• Highlights importance of **testing assumptions**  
• Provides framework for **marketing ROI evaluation**  

### 💡 Business Value  
📌 **For CFOs:**  
   - Evidence for budget allocation decisions  
   - Identifies weak spending-revenue linkages  

📌 **For Marketing Teams:**  
   - Guides campaign optimization strategies  
   - Supports case for testing alternative channels  

📌 **For Data Teams:**  
   - Complete correlation analysis template  
   - Assumption validation best practices  

### 📈 Statistical Approach  
1. **Assumption Verification:**  
   - Normality (Shapiro-Wilk p = 0.6552 & 0.2083)  
   - Homogeneity (Levene's p < 0.001)  

2. **Pearson Correlation Results:**  
   - r = 0.0545 (Very weak positive)  
   - p-value = 0.5904  
   - 95% CI: [-0.14, 0.24]  

### 🔑 Key Findings  
• **Statistically Insignificant** relationship (p > 0.05)  
• **Negligible Effect Size** (r < 0.1)  
• Only **5.4% of revenue variance** explained by ad spend  

### 📢 Strategic Conclusion  

**No significant linear relationship exists between advertising spend and revenue (p = 0.59). Businesses should:**  
1️⃣ **Investigate other revenue drivers**  
2️⃣ **Optimize existing campaigns before increasing budgets**  
3️⃣ **Test alternative marketing channels**


---

### 7. Mann-Whitney U Test

📄 **Project Link:** **[Mann-Whitney U Test.ipynb](Hypothesis%20Testing/Hypothesis%20Tests/5.%20Mann-Whitney%20U%20Test.ipynb)**

## 📊 **Non-Parametric Comparison: North vs South Sales Performance**  

### 🌟 Overview  
This project employs the **Mann-Whitney U Test** to compare sales revenue distributions between two retail regions without normality assumptions. Using synthetic gamma-distributed data, we demonstrate proper non-parametric analysis workflow from assumption checks to business interpretation.

### ❓ Problem Statement  
"Is there a statistically significant difference in sales performance between our North and South regions, given non-normal revenue distributions?"  

### 🎯 Objective  
• Compare regional sales distributions robustly  
• Demonstrate non-parametric testing methodology  
• Guide regional strategy decisions with data  

### 📊 Dataset Description  
**Synthetic Revenue Data (200 Records):**  
• **North Region (100 stores):**  
  - Gamma distribution (shape=2, scale=500)  
  - Positively skewed  
• **South Region (100 stores):**  
  - Gamma distribution (shape=2, scale=520)  
  - Slightly higher potential values  

**Variables:**  
• `region`: Categorical (North/South)  
• `revenue`: Continuous numerical values  

### 🚀 Project Highlights  
✅ **Proper Assumption Handling:**  
   - Confirmed non-normality (Shapiro-Wilk p < 0.001)  
   - Verified equal variances (Levene's p = 0.198)  

✅ **Robust Statistical Testing:**  
   - Correct application of Mann-Whitney U test  
   - Clear interpretation of rank-based comparison  

✅ **Actionable Business Insights:**  
   - Translates statistical results to strategic guidance  
   - Provides framework for regional performance analysis  

### 🔍 Why This Matters  
• Real-world demonstration of **non-parametric testing**  
• Shows alternative when t-test assumptions fail  
• Provides template for **skewed data comparisons**  

### 💡 Business Value  
📌 **For Regional Managers:**  
   - Evidence-based performance evaluation  
   - Avoids misleading normal-distribution assumptions  

📌 **For Data Teams:**  
   - Complete non-parametric analysis example  
   - Proper assumption validation techniques  

📌 **For Executives:**  
   - Confidence in regional comparisons  
   - Guides resource allocation decisions  

### 📈 Statistical Approach  
1. **Assumption Verification:**  
   - Shapiro-Wilk: Confirmed non-normality (p < 0.001)  
   - Levene's Test: Equal variances (p = 0.198)  

2. **Mann-Whitney U Test Results:**  
   - U-statistic: 4549.0  
   - p-value: 0.2710  
   - Effect Size: Rank-biserial correlation optional  

### 🔑 Key Findings  
• **High p-value (0.271 > 0.05)** → Fail to reject null  
• **No significant difference** in revenue distributions  
• Median revenues:  
  - North: $963.42  
  - South: $996.87  

### 📢 Strategic Conclusion  

**No statistically significant difference exists between North and South sales distributions (p = 0.27). Regional strategies should:** 

1️⃣ **Focus on non-geographic performance drivers**
2️⃣ **Investigate higher-level business factors**  
3️⃣ **Maintain consistent policies across regions**


---

## 8. Wilcoxon Signed-Rank Test

📄 **Project Link:** **[Wilcoxon Signed-Rank Test.ipynb](Hypothesis%20Testing/Hypothesis%20Tests/6.%20Wilcoxon%20Signed-Rank%20Test.ipynb)**

## 📈 Wilcoxon Signed-Rank Test: Promotional Campaign Impact Analysis  

### 🌟 Overview  
This project applies the **Wilcoxon Signed-Rank Test** to evaluate whether a promotional campaign significantly increased daily sales. Using synthetic paired data that violates normality assumptions, we demonstrate proper non-parametric analysis for before-after studies.

### ❓ Problem Statement  
"Did our recent promotional campaign actually increase sales, given that our sales data isn't normally distributed?"  

### 🎯 Objective  
• Quantify campaign impact without normality assumptions  
• Demonstrate robust paired data analysis  
• Provide actionable marketing insights  

### 📊 Dataset Description  
**Synthetic Sales Data (60 Days):**  
• **Before Campaign:**  
  - Gamma distribution (shape=2, scale=100)  
  - Median: $191.42  
• **After Campaign:**  
  - Before sales + N(10,15) boost  
  - Median: $200.87 (+4.9%)  

**Variables:**  
• `before_sales`: Daily sales pre-campaign  
• `after_sales`: Daily sales post-campaign  

### 🚀 Project Highlights  
✅ **Assumption Validation:**  
   - Confirmed non-normality of differences (Shapiro-Wilk p=0.295)  
   - Proper handling of paired observations  

✅ **Robust Statistical Testing:**  
   - Correct application of Wilcoxon signed-rank test  
   - Effect size calculation (optional)  

✅ **Business-Ready Insights:**  
   - Clear interpretation of median differences  
   - Statistical significance with practical implications  

### 🔍 Why This Matters  
• Real-world demonstration of **non-parametric paired testing**  
• Shows alternative when paired t-test assumptions fail  
• Provides template for **marketing intervention analysis**  

### 💡 Business Value  
📌 **For Marketing Teams:**  
   - Proof of campaign effectiveness  
   - Justification for future promotions  

📌 **For Store Managers:**  
   - Quantified sales impact  
   - Benchmark for future initiatives  

📌 **For Data Teams:**  
   - Complete non-parametric workflow  
   - Best practices for skewed paired data  

### 📈 Statistical Approach  
1. **Assumption Verification:**  
   - Shapiro-Wilk on differences (p=0.295 → non-normal)  

2. **Wilcoxon Signed-Rank Results:**  
   - Test Statistic: 309.0  
   - p-value: <0.001  
   - Median Increase: +$9.45 (4.9%)  

### 🔑 Key Findings  
• **Highly Significant Result** (p < 0.0001)  
• **Median Sales Increase**: +4.9%  
• **Practical Impact**: Campaign successfully boosted sales  

### 📢 Executive Conclusion  
**The promotional campaign **significantly increased daily sales** by a median of 4.9% (p < 0.001). This strong evidence supports:**  
1️⃣ **Repeating similar campaigns**  
2️⃣ **Allocating budget for promotions**  
3️⃣ **Further testing to optimize impact**

---

## 9. Kruskal-Wallis Test

📄 **Project Link:** **[Kruskal-Wallis Test](Hypothesis%20Testing/Hypothesis%20Tests/7.%20Kruskal-Wallis%20Test.ipynb)**

## 📊 **Kruskal-Wallis Test: Comparing Marketing Channel Performance**  

### 🌟 Overview  
This project applies the **Kruskal-Wallis H-test** to evaluate whether sales performance differs across three marketing channels (Email, Social Media, TV) when data violates normality assumptions. The analysis provides robust insights for marketing budget allocation decisions.

### ❓ Problem Statement  
"Do our marketing channels (Email vs Social Media vs TV) generate significantly different sales results, given non-normal revenue distributions?"  

### 🎯 Objective  
• Compare channel performance without normality assumptions  
• Demonstrate proper non-parametric multi-group analysis  
• Guide marketing budget allocation decisions  

### 📊 Dataset Description  
**Synthetic Sales Data (150 Records):**  
• **Email Campaign (50):**  
  - Gamma distribution (shape=2, scale=120)  
  - Median: $229.18  
• **Social Media (50):**  
  - Gamma distribution (shape=2, scale=110)  
  - Median: $210.65  
• **TV Campaign (50):**  
  - Gamma distribution (shape=2, scale=140)  
  - Median: $268.94  

**Variables:**  
• `channel`: Categorical (Email/Social/TV)  
• `sales`: Continuous numerical values  

### 🚀 Project Highlights  
✅ **Comprehensive Assumption Checks:**  
   - Confirmed non-normality for all channels (Shapiro-Wilk p < 0.05)  
   - Verified ordinal data structure  

✅ **Robust Statistical Testing:**  
   - Correct application of Kruskal-Wallis test  
   - Post-hoc analysis available if significant  

✅ **Actionable Business Insights:**  
   - Clear interpretation of median sales  
   - Statistical significance with practical implications  

### 🔍 Why This Matters  
• Real-world demonstration of **non-parametric ANOVA alternative**  
• Shows proper handling of **skewed multi-group data**  
• Provides template for **marketing channel evaluation**  

### 💡 Business Value  
📌 **For CMOs:**  
   - Data-driven channel performance assessment  
   - Objective budget allocation guidance  

📌 **For Marketing Teams:**  
   - Identifies equally effective channels  
   - Prevents over-investment in underperforming channels  

📌 **For Data Teams:**  
   - Complete non-parametric workflow  
   - Best practices for ordinal data analysis  

### 📈 Statistical Approach  
1. **Assumption Verification:**  
   - Shapiro-Wilk tests (All p < 0.05 → non-normal)  

2. **Kruskal-Wallis Test Results:**  
   - H-statistic: 2.6024  
   - p-value: 0.2722  
   - Group Medians:  
     • Email: $229.18  
     • Social: $210.65  
     • TV: $268.94  

### 🔑 Key Findings  
• **High p-value (0.272 > 0.05)** → Fail to reject null  
• **No significant difference** in sales distributions  
• Observed median differences likely due to random variation  

### 📢 Strategic Conclusion  
**All three marketing channels perform **statistically similarly** in sales generation (p = 0.27). Recommendations:**  
1️⃣ **Allocate budgets based on cost-efficiency rather than sales differences**  
2️⃣ **Investigate other performance metrics (ROI, customer acquisition cost)**  
3️⃣ **Consider testing additional channels or campaign variations**

---

## 10. Chi-Square Goodness of Fit Test

📄 **Project Link:** **[Chi-Square Goodness.ipynb
](Hypothesis%20Testing/Hypothesis%20Tests/8.%20Chi-Square%20Goodness.ipynb)**

📊 Chi-Square Goodness of Fit: Marketing Campaign Analysis  

### 🌟 Overview  
This project applies the **Chi-Square Goodness of Fit Test** to evaluate whether observed customer responses across three marketing campaigns match expected historical patterns. The analysis helps validate marketing channel performance assumptions.

### ❓ Problem Statement  
"Does our current customer response distribution across Email, Social Media, and TV campaigns differ significantly from what we historically expect?"  

### 🎯 Objective  
• Test alignment between observed and expected customer distributions  
• Demonstrate proper Chi-Square Goodness of Fit implementation  
• Provide data-driven insights for campaign evaluation  

### 📊 Dataset Description  
**Synthetic Customer Response Data:**  
• **Observed Counts:**  
  - Email: 120 customers  
  - Social Media: 95 customers  
  - TV: 85 customers  
• **Expected Proportions:**  
  - Email: 40%  
  - Social Media: 35%  
  - TV: 25%  

**Total Customers:** 300  

### 🚀 Project Highlights  
✅ **Proper Test Selection:**  
   - Designed for categorical frequency data  
   - Non-parametric (no normality assumptions)  

✅ **Rigorous Assumption Checks:**  
   - Verified expected frequencies ≥5  
   - Confirmed independence of observations  

✅ **Clear Interpretation:**  
   - Business-focused conclusions  
   - Practical significance assessment  

### 🔍 Why This Matters  
• Demonstrates **distribution validation** technique  
• Provides framework for **marketing performance benchmarking**  
• Shows proper **categorical data analysis** approach  

### 💡 Business Value  
📌 **For Marketing Teams:**  
   - Validates campaign performance assumptions  
   - Guides resource allocation decisions  

📌 **For Data Analysts:**  
   - Complete Chi-Square workflow example  
   - Expected frequency calculation method  

📌 **For Executives:**  
   - Confidence in campaign distribution patterns  
   - Evidence for strategic planning  

### 📈 Statistical Approach  
1. **Assumption Verification:**  
   - All expected counts ≥5 (Met)  
   - Independent observations (By design)  

2. **Chi-Square Test Results:**  
   - χ² Statistic: 2.2857  
   - p-value: 0.3189  
   - Degrees of Freedom: 2  

### 🔑 Key Findings  
• **High p-value (0.319 > 0.05)** → Fail to reject null  
• **No significant difference** between observed/expected  
• Current campaign responses match historical patterns  

### 📢 Strategic Conclusion  
**Customer responses align with historical distributions across all channels (p = 0.32). Recommended actions:**  
1️⃣ **Maintain current campaign mix**  
2️⃣ **Monitor for future deviations**  
3️⃣ **Investigate absolute performance metrics**

---

### 🛠️ Technical Implementation  
   - Python (Pandas, NumPy)  
   - SciPy (kruskal, shapiro)  
   - Matplotlib/Seaborn (Visualizations)


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

