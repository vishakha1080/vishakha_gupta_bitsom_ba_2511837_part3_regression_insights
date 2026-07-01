\# Model Comparison

\## Overview

Two regression models were developed to understand the factors associated with monthly sales performance across retail stores.

\---

\## Model 1: Simple Linear Regression

\### Dependent Variable

Monthly Sales

\### Independent Variable

Marketing Spend

\### Results

| Metric | Value |

|----------|----------|

| R Square | 0.1672 |

| Adjusted R Square | 0.1646 |

| Coefficient | 2.1296 |

| P-value | 2.48E-14 |

\### Interpretation

The model indicates that marketing spend has a positive and statistically significant relationship with monthly sales. For every one-unit increase in marketing spend, monthly sales increase by approximately 2.13 units on average.

However, the model explains only 16.7% of the variation in monthly sales, indicating that additional business factors influence store performance.

\### Strengths

\- Easy to interpret

\- Statistically significant

\- Useful for understanding the impact of marketing spend

\### Limitations

\- Ignores store traffic, inventory availability, and regional differences

\- Limited explanatory power

\---

\## Model 2: Multiple Regression

\### Dependent Variable

Monthly Sales

\### Independent Variables

\- Marketing Spend

\- Footfall

\- Average Discount Percentage

\- Inventory Availability Percentage

\- North Region Dummy

\- South Region Dummy

\- West Region Dummy

\### Results

| Metric | Value |

|----------|----------|

| R Square | 0.8127 |

| Adjusted R Square | 0.8085 |

\### Significant Variables

\- Marketing Spend

\- Footfall

\- Inventory Availability Percentage

\- South Region Dummy

\- West Region Dummy

\### Interpretation

The multiple regression model explains approximately 81.3% of the variation in monthly sales. This represents a substantial improvement over the simple regression model.

The results suggest that customer traffic, marketing investment, inventory availability, and regional differences are important drivers of sales performance.

\### Strengths

\- High explanatory power

\- Includes multiple business drivers

\- More useful for managerial decision-making

\### Limitations

\- Does not include seasonal trends

\- Does not account for local competition

\- Cannot establish causation

\---

\## Final Model Selection

The Multiple Regression Model was selected as the final model because it achieved the highest explanatory power (R² = 0.8127) and provided more comprehensive business insights than the simple regression model.