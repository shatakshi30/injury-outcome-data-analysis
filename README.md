# Injury Outcome Data Analysis

This project applies statistical techniques to analyze injury outcomes using demographic, clinical, and self-reported variables. The work was conducted as the final project for the *Statistical Methods and Data Analysis* course.

---

## Dataset

- **Source**: Real-world dataset on injuries suffered by children and adolescents.
- **Samples**: 203 observations, ages 8–18 years.
- **Variables**: 19 variables covering demographics (Age, Sex, Race), injury characteristics (Injury Type, Injury Duration), healthcare usage (Care Site), and patient-reported outcomes (Rating2).

---

## Objectives

- Explore predictors of **Injury Duration** using demographic and clinical variables.
- Investigate the association between **Injury Type** and **Injury Duration**, moderated by **Age** and **Sex**.
- Assess the predictive power of **Rating2** on **Injury Duration**.
- Analyze how **Age** influences the choice of **Care Site** (e.g., Emergency Care vs. Primary Care).
- Provide visualizations and statistical summaries to support the findings.

---

## Methods

- **Data Cleaning**: Median/mode imputation for missing values.
- **Descriptive Statistics**: Summary tables and distributions.
- **Linear Regression**:
  - Injury Duration ~ Injury Type + Age + Sex + Interactions
  - Injury Duration ~ Rating2
- **Logistic Regression**:
  - Binary outcome for Care Site (Emergency vs. Others) ~ Age Group
- **Correlation Analysis**: Pearson correlation between Rating2 and Injury Duration.
- **Model Diagnostics**: Residual plots, ROC curves for logistic regression.

---

## Key Findings

1. **Injury Type and Injury Duration**:
   - Sport-related injuries significantly associated with longer recovery times.
   - Interaction between Sport Injury and Age approached significance.

2. **Patient-Reported Outcomes (Rating2)**:
   - Significant negative correlation with Injury Duration (p < 0.0001).
   - Higher patient ratings → faster recovery.

3. **Healthcare Utilization (Care Site)**:
   - Younger patients (8–12 years) more likely to visit Emergency Care than older adolescents (15–18 years).

4. **Model Summaries**:
   - Linear model explained 17.7% of variation in Injury Duration.
   - Logistic regression AUC = 0.639, indicating modest predictive performance.

---

## How to Run

### Requirements

- R >= 4.0
- RStudio recommended
- Required R packages:
```r
install.packages("tidyverse")
install.packages("ggplot2")
install.packages("broom")
install.packages("pROC")
```

## 📁 Files in this Repository
injury_outcome_analysis.Rmd → Full analysis pipeline (R Markdown)

Injury_Data.csv → Dataset used for the analysis

injury_outcome_analysis(knitted report).docx → Knitted report (Word format)

Data Analysis Project Report.pdf → Final report document

## Learnings
Applied linear and logistic regression to real-world healthcare data.

Gained hands-on experience in hypothesis testing, correlation analysis, and model evaluation.

Developed and validated statistical models with real-world healthcare applications.

Enhanced proficiency in R and statistical modeling for health data analysis.
