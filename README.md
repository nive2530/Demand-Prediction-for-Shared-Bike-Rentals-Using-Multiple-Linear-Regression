# Demand-Prediction-for-Shared-Bike-Rentals-Using-Multiple-Linear-Regression

## Project Objective
To develop a robust multiple linear regression model for predicting the daily demand for shared bikes. This model aims to identify significant factors influencing bike demand and provide actionable insights to optimize operations, improve customer satisfaction, and maximize revenue for a bike-sharing service provider.

## Problem Statement
BoomBikes, a US-based bike-sharing provider, seeks to understand the factors influencing bike rental demand to adjust their business strategy post-pandemic. The primary goals are:
- Identifying significant predictors of bike demand.
- Quantifying the relationship between demand and influencing variables.
  
The analysis will support the company in forecasting demand and tailoring their services to meet customer needs effectively.

## Key Tasks and Technical Details
**1. Data Preparation** 
  **Data Cleaning:**
      - Handled missing values and outliers to ensure data consistency and reliability.
      - Analyzed numerical and categorical variables for discrepancies.
  
  **Feature Engineering:**
      - Converted ordinal variables (e.g., season, weathersit) into categorical labels using one-hot encoding to remove implicit hierarchy.
      - Retained the yr variable, identifying it as a valuable predictor due to increasing bike-sharing popularity over time.

  **Scaling and Transformation:**
      - Normalized continuous variables like temp, hum, and windspeed using Min-Max scaling to improve model interpretability and convergence.

**2. Exploratory Data Analysis (EDA)**
**Univariate Analysis:**
- Analyzed distributions of individual features using histograms and box plots to identify trends and anomalies.
**Bivariate and Multivariate Analysis:**
- Correlation heatmaps identified key relationships between independent variables and the target variable cnt.
- Scatter plots and pair plots highlighted multicollinearity and potential predictors for the regression model.

**3. Model Building**
**Target Variable:**
- Modeled cnt (total bike demand) as the dependent variable, summing casual and registered users.
**Multiple Linear Regression:**
- Built the regression model using Python's sklearn library.
- Addressed multicollinearity using Variance Inflation Factor (VIF) analysis to select features contributing to prediction accuracy.
- Implemented a stepwise feature selection process to optimize the model.

**4. Model Evaluation**
**Residual Analysis:**
- Analyzed residual plots to ensure that assumptions of linearity, homoscedasticity, and normality were met.
**Performance Metrics:**
- Evaluated the model using R-squared and Adjusted R-squared values.
- Used the r2_score metric to assess predictive accuracy on test data.

## Tools and Technologies Used

**Programming Language:** Python
**Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels
**Techniques:**
- One-hot encoding, feature scaling, and VIF for multicollinearity assessment.
- Model diagnostics for evaluating residuals and performance metrics.

## Key Insights and Outcomes
- Identified key predictors of bike demand, such as temperature, humidity, and weather conditions.
- Established a clear seasonal trend, with higher demand during summer and fall.
- Validated the model with an R-squared score, confirming its suitability for forecasting bike demand.

## Conclusion
This project successfully delivered a predictive model for shared bike demand, providing actionable insights for BoomBikes to optimize their operations and plan for post-pandemic growth.
