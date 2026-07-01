\# Model Equations

\## Simple Regression Model

\### Equation

Monthly Sales = 560777.35 + 2.1296(Marketing Spend)

\---

\### Interpretation

The coefficient of 2.1296 indicates that higher marketing spend is associated with higher monthly sales.

The positive coefficient and statistically significant p-value suggest that marketing investment contributes positively to sales performance.

R² = 0.1672

This means that marketing spend alone explains approximately 16.7% of the variation in monthly sales.

\---

\# Multiple Regression Model

\## Equation

Monthly Sales =

144334.52

\+ 1.1751(Marketing Spend)

\+ 33.8478(Footfall)

− 55735.82(Avg Discount Percentage)

\+ 2764.37(Inventory Availability Percentage)

\+ 10603.68(North)

\+ 20145.99(South)

\+ 17060.36(West)

\---

\## Coefficient Interpretation

\### Marketing Spend

Coefficient: 1.1751

A higher marketing budget is associated with increased monthly sales after controlling for other variables.

\---

\### Footfall

Coefficient: 33.8478

Stores with higher customer traffic tend to generate higher monthly sales.

This is one of the strongest predictors in the model.

\---

\### Average Discount Percentage

Coefficient: -55735.82

The coefficient is negative, suggesting that larger discounts may be associated with lower sales after controlling for other variables.

However, the p-value is not statistically significant, so this relationship should be interpreted cautiously.

\---

\### Inventory Availability Percentage

Coefficient: 2764.37

Stores with better inventory availability tend to achieve higher monthly sales.

This variable is statistically significant.

\---

\## Dummy Variables

\### Reference Category

East Region

East was selected as the reference category to avoid the dummy variable trap.

\---

\### North Dummy

1 = North Region

0 = Otherwise

Coefficient: 10603.68

Represents the expected sales difference between North and East stores.

Not statistically significant.

\---

\### South Dummy

1 = South Region

0 = Otherwise

Coefficient: 20145.99

South region stores generate higher sales than East region stores on average.

Statistically significant.

\---

\### West Dummy

1 = West Region

0 = Otherwise

Coefficient: 17060.36

West region stores generate higher sales than East region stores on average.

Statistically significant.

\---

\# Final Model Selected

Multiple Regression Model

\## Reason for Selection

The multiple regression model achieved:

\- R² = 0.8127

\- Adjusted R² = 0.8085

The model explains more than 81% of the variation in monthly sales and provides actionable business insights regarding marketing investment, customer traffic, inventory management, and regional performance.