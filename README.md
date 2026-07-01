# Regression-Based Business Insights & Model Interpretation

## Business Problem

A retail chain wants to understand which factors are most strongly associated with monthly sales performance across stores. Leadership is considering actions such as increasing marketing spend, improving inventory availability, adjusting discount strategies, and prioritizing specific regions.

The objective of this project is to use regression analysis to identify key sales drivers and provide data-driven business recommendations.

---

# Dataset Description

The dataset contains store-level operational and performance metrics for 320 observations.

Variables available include:

- Monthly Sales
- Marketing Spend
- Footfall
- Average Discount Percentage
- Staff Count
- Inventory Availability Percentage
- Competitor Distance
- Customer Rating
- Region
- Store Type

---

# Dependent Variable

The dependent variable used in all regression models is:

**Monthly Sales**

---

# Independent Variables

The following variables were considered as potential predictors:

- Marketing Spend
- Footfall
- Average Discount Percentage
- Inventory Availability Percentage
- Staff Count
- Customer Rating
- Competitor Distance
- Region

---

# Variable Classification

## Numerical Variables

- Monthly Sales
- Marketing Spend
- Footfall
- Average Discount Percentage
- Staff Count
- Inventory Availability Percentage
- Competitor Distance
- Customer Rating

## Categorical Variables

- Region
- Store Type

---

# Data Preparation

The dataset was reviewed before analysis.

Data preparation activities included:

- Checking for missing values
- Reviewing numerical and categorical variables
- Checking for duplicate records
- Creating dummy variables for categorical variables
- Preparing data for regression analysis

---

# Dummy Variable Approach

The categorical variable **Region** was converted into dummy variables.

Dummy Variables Created:

- North
- South
- West

Reference Category:

**East Region**

East was selected as the reference category to avoid multicollinearity and the dummy variable trap.

Interpretation:

- North = 1 if store belongs to North region, otherwise 0
- South = 1 if store belongs to South region, otherwise 0
- West = 1 if store belongs to West region, otherwise 0

---

# Regression Approach

Two regression models were developed.

## Model 1: Simple Regression

Dependent Variable:

- Monthly Sales

Independent Variable:

- Marketing Spend

### Results

| Metric | Value |
|----------|----------|
| R Square | 0.1672 |
| Coefficient | 2.1296 |
| P-value | 2.48E-14 |

### Interpretation

Marketing spend has a positive and statistically significant relationship with monthly sales. However, the model explains only 16.7% of the variation in sales.

---

## Model 2: Multiple Regression

Dependent Variable:

- Monthly Sales

Independent Variables:

- Marketing Spend
- Footfall
- Average Discount Percentage
- Inventory Availability Percentage
- North Dummy
- South Dummy
- West Dummy

### Results

| Metric | Value |
|----------|----------|
| R Square | 0.8127 |
| Adjusted R Square | 0.8085 |

### Significant Variables

- Marketing Spend
- Footfall
- Inventory Availability Percentage
- South Region
- West Region

### Interpretation

The model explains approximately 81.3% of the variation in monthly sales and provides stronger business insights than the simple regression model.

---

# Model Comparison Summary

| Model | R Square | Business Usefulness |
|---------|---------|---------|
| Simple Regression | 0.1672 | Limited explanatory power |
| Multiple Regression | 0.8127 | Strong decision-making model |

The multiple regression model substantially outperformed the simple regression model and was selected as the final model.

---

# Final Model Selected

## Multiple Regression Model

Reason for Selection:

- Highest R² value (0.8127)
- Strong explanatory power
- Includes multiple business drivers
- Provides actionable business recommendations

---

# Key Business Insights

1. Footfall is the strongest predictor of monthly sales.
2. Marketing spend has a positive and significant impact on sales.
3. Inventory availability contributes positively to sales performance.
4. South and West regions outperform the East region.
5. Average discount percentage is not statistically significant and should be interpreted cautiously.

---

# Business Recommendation

Leadership should prioritize:

- Increasing customer footfall
- Maintaining effective marketing investments
- Improving inventory availability
- Studying successful practices in South and West regions

Discount strategies should not be considered the primary driver of sales growth based on the regression results.

---

# Assumptions and Limitations

The analysis has several limitations:

- Regression identifies association, not causation.
- Seasonal demand patterns were not included.
- Local competition was not included.
- Economic and demographic factors were not included.
- Some store-specific influences may remain unexplained.

Future analyses could incorporate additional variables to improve predictive accuracy.

---

# Residual Analysis Summary

Residual analysis was conducted using the final multiple regression model.

Key observations:

- Positive residuals indicate stores performing better than predicted.
- Negative residuals indicate stores performing worse than predicted.
- The model explains approximately 81.3% of sales variation, indicating strong predictive performance.
- Some unexplained variation remains, suggesting that additional factors may influence store sales.

---

# Screenshots Included

The repository includes the following screenshots:

- simple_regression_output.png
- multiple_regression_output.png
- residuals_preview.png
- model_comparison_preview.png

---

# Repository Structure

part3_regression_insights/

├── data/

│ └── business_regression_data.xlsx

├── analysis/

│ ├── regression_workbook.xlsx

│ ├── model_comparison.md

│ └── residual_analysis.md

├── outputs/

│ ├── regression_summary.xlsx

│ ├── final_recommendation.md

│ └── model_equations.md

├── screenshots/

│ ├── simple_regression_output.png

│ ├── multiple_regression_output.png

│ ├── residuals_preview.png

│ └── model_comparison_preview.png

└── README.md
