Advertising Sales Prediction
1. Project Overview

This project uses Machine Learning to predict product sales based on advertising expenditure.

The dataset contains advertising spending on:

TV
Radio
Newspaper

The target variable is Sales.

2. Objectives
Analyze the advertising dataset
Identify the input features and target variable
Build a Multiple Linear Regression model
Train the model using historical data
Predict sales for unseen data
Evaluate the model performance
Identify the advertising channel with the strongest impact
Provide a business recommendation

3. Dataset
The dataset contains 200 rows and 4 columns.

Column	Description
TV	Advertising budget spent on TV
Radio	Advertising budget spent on Radio
Newspaper	Advertising budget spent on Newspaper
Sales	Product sales

Input Features: TV, Radio, Newspaper
Target Variable: Sales

4. Technologies Used
Python
Pandas
NumPy
Matplotlib
Scikit-learn
Jupyter Notebook

5. Project Workflow
Load the dataset
Explore the dataset
Check for missing values
Select input features and target
Split the data into training and testing sets
Train the Linear Regression model
Make predictions
Evaluate the model
Interpret the results
Provide business recommendations

6. Data Preparation
The input features are:

X = df[["TV", "Radio", "Newspaper"]]

The target variable is:

y = df["Sales"]

The dataset was divided into:

80% Training Data
20% Testing Data

No missing values were found in the dataset.

7. Machine Learning Model
Multiple Linear Regression

The model learns the relationship between advertising expenditure and Sales.

The general equation is:

Sales = Intercept + (TV × TV Coefficient)
                 + (Radio × Radio Coefficient)
                 + (Newspaper × Newspaper Coefficient)
Model Coefficients
Feature	Coefficient
TV	0.054509
Radio	0.100945
Newspaper	0.004337
Intercept	4.714126

8. Model Evaluation
The model was evaluated using the following metrics:

Metric	Result
MAE	1.275
MSE	2.908
RMSE	1.705
R² Score	0.906

The model achieved an R² score of approximately 90.6%.

9. Sales Prediction
The model was used to predict Sales for the following advertising budget:

TV = 150
Radio = 20
Newspaper = 30
Predicted Sales
15.04

10. Key Findings
Radio has the strongest estimated impact on Sales.
TV has a positive impact on Sales.
Newspaper has the least estimated impact.
The model achieved an R² score of 0.906.
The model predicted approximately 15.04 Sales for the given budget.

11. Business Recommendation
Based on the model results, the company should prioritize Radio advertising because it has the strongest estimated impact on Sales.

The company can also review Newspaper advertising expenditure and consider reallocating some of the budget toward higher-impact channels.

12. Technical Improvement
The current model uses Multiple Linear Regression.

Future improvements can include:

Random Forest Regression
Gradient Boosting
Cross-Validation
Hyperparameter Tuning
Feature Engineering