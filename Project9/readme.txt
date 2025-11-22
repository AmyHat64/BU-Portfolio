Overview

This project explores how demographic and lifestyle factors influence health insurance charges. Using a dataset of 1,338 individuals, the goal is to identify the key drivers of medical insurance costs and build models that can predict charges more accurately. The project applies regression, classification, and clustering techniques to uncover patterns and test the predictive power of various features such as age, BMI, smoking status, and region.

Dataset

The dataset (insurance.csv) includes:

Age

Sex

BMI (Body Mass Index)

Number of children/dependents

Smoking status

Region

Annual medical charges (target variable)

The data contains no missing values and reflects common underwriting variables used in real-world insurance pricing.

Methods

The workflow includes:

Exploratory Data Analysis (EDA): Histograms, scatterplots, boxplots, and a correlation heatmap (see page 4–6)

Encoding: Converting categorical variables (sex, smoker, region) to numeric form

Regression Models:

Linear Regression

Random Forest Regressor

Gradient Boosting Regressor

Classification Models: Logistic Regression and Random Forest to attempt predicting smoker status

Clustering: K-Means clustering (k = 2–4) to identify natural groupings in the population

Model performance was evaluated using RMSE, MAE, R² for regression, and accuracy/F1 score for classification.

Results

Smoking status was the strongest predictor of high insurance charges.

Boxplots on page 4 show smokers’ charges can exceed $60,000, while non-smokers remain much lower.

Best Regression Model: Gradient Boosting

RMSE ≈ 4,330

R² ≈ 0.88

Feature importance: Smoking, BMI, and age had the highest influence on predicted charges.

Classification: Predicting smoking status based on other features performed poorly, indicating weak signal.

Clustering: K-Means successfully isolated high-cost smoker groups as shown in the cluster centers on page 8.

Overall, lifestyle variables—especially smoking—dominate cost variation, while region and sex contribute minimally.

Tools

Python

pandas

scikit-learn

seaborn & matplotlib

Jupyter Notebook

Future Work

Add medical history, activity level, occupation, or wearable data

Implement SHAP/LIME for explainability

Explore time-series modeling of recurring medical costs

Build dashboards for underwriting teams

Expand to usage-based or behavior-based pricing frameworks
