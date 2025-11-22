
Overview

This project explores how everyday habits—such as screen time, social media use, sleep quality, and exercise—relate to self-reported stress levels. Using survey data from 500 participants, the goal is to build predictive models that estimate stress and identify which behaviors influence it the most. This work supports the growing need to understand digital well-being and how modern lifestyle patterns affect mental health.

Dataset

The dataset (from Kaggle, 2023) includes approximately 500 individuals with the following variables:

Age

Gender

Daily screen time

Sleep quality (1–10)

Stress level (1–10, target)

Days without social media

Exercise frequency

Primary social media platform

Happiness index

The dataset contained no missing values, and categorical fields (e.g., gender, platform) were encoded numerically for modeling.

Methods

The analysis consisted of several steps:

Exploratory Data Analysis

Histograms of all numeric features (page 4)

Correlation heatmap (page 5) showing strong relationships between screen time, sleep, happiness, and stress

Boxplots comparing stress by gender and social media platform (page 5–6)

Modeling

Three regression models were tested using an 80/20 train-test split:

Linear Regression

Random Forest Regressor

Gradient Boosting Regressor

Categorical variables were processed via OneHotEncoder, and all models were built inside scikit-learn pipelines.

Model evaluation metrics included MAE, RMSE, and R².

Results

The Random Forest model performed best:

Model	MAE	RMSE	R²
Random Forest	0.80	0.94	0.63
Gradient Boosting	0.81	0.96	0.62
Linear Regression	0.81	0.97	0.61

Key findings from the analysis:

Higher daily screen time strongly correlates with higher stress.

Better sleep quality is linked to lower stress.

Exercise and social media platform showed weaker relationships.

Happiness index had a strong negative correlation with stress (page 5 heatmap).

These results confirm that sleep and digital habits are major contributors to perceived stress.

Tools

Python

pandas

scikit-learn

seaborn & matplotlib

Jupyter Notebook

Future Work

Integrate additional mental-health variables like anxiety or burnout scores

Incorporate longitudinal data to track stress over time

Build real-time wellness recommendation systems

Add explainability tools (SHAP, LIME) to understand model predictions
