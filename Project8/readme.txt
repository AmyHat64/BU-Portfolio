Overview

This project builds a machine learning model to predict auto insurance premiums using a dataset of 1,000 drivers. The goal is to understand which factors—such as age, driving experience, accident history, vehicle age, and mileage—most strongly influence insurance pricing, and to develop a predictive model that can accurately estimate a customer’s premium.

Dataset

The dataset includes 1,000 records, each describing a driver and their associated premium. Features include:

Driver Age

Driving Experience

Previous Accidents

Annual Mileage

Car Manufacturing Year

Car Age

Insurance Premium (target)

The dataset contains no missing values and consists entirely of numeric fields, which simplifies preprocessing. Car Age and Manufacturing Year were perfectly correlated, so only one was required for modeling.

Methods

The project begins with exploratory data analysis (EDA), including:

Histograms for distribution visualization (page 3–8)

Boxplots to identify outliers (page 10–15)

A correlation heatmap showing relationships among variables (page 16–17)

Scatterplot of premium vs. driving experience (page 18)

A preprocessing pipeline was built using ColumnTransformer, StandardScaler, and imputers. Several regression models were trained and tested:

Linear Regression

Ridge Regression (RidgeCV)

Random Forest Regressor

Gradient Boosting Regressor

Results

After evaluating RMSE, MAE, and R² scores, the Linear Regression model delivered the best results, with an RMSE extremely close to zero and an R² of 1.0, indicating a near-perfect fit for this dataset.

Visuals such as the correlation heatmap show that:

Premiums decrease sharply with driver age and driving experience

Accident history increases premiums

Car age and mileage have minimal impact

These findings match established insurance industry research.

A residual plot (page 20) confirms linearly distributed errors, supporting the model’s accuracy.

Tools

Python

pandas

scikit-learn

seaborn / matplotlib

joblib (model saving)

Jupyter Notebook

Future Work

Add telematics data (speed, braking, time of day)

Incorporate geographic and demographic variables

Train additional models on larger datasets

Explore fairness concerns and mitigate bias

Develop real-time usage-based pricing prototypes

Summary

This project shows that driver-related variables—especially age, experience, and accident history—are the strongest predictors of insurance premiums. The final Linear Regression model performs extremely well on the dataset and demonstrates how machine learning can supplement or improve traditional actuarial rating methods.
