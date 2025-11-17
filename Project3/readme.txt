Predicting Mental Health Outcomes from Music Preferences
Overview
This project examines whether music preferences can predict mental health outcomes using machine learning models. A Kaggle dataset of survey responses connects musical habits with self-reported mental health conditions.
Dataset
•	Kaggle MXMH survey dataset (736 responses)
•	Features: favorite genres, listening hours, streaming services, demographics
•	Targets: depression, anxiety, OCD, insomnia
Methods
•	Exploratory data analysis (EDA)
•	Data cleaning (renaming columns, handling missing values)
•	Machine learning models: Naive Bayes, KNN, Decision Tree
Results
•	Naive Bayes: 76% accuracy
•	KNN: 81% accuracy (after tuning)
•	Decision Tree: 98% accuracy but possible overfitting
•	Certain genres correlated with mental health outcomes (e.g., lo-fi linked with higher depression, gospel linked with reduced anxiety)
Tools
Python, pandas, scikit-learn, Matplotlib
Future Work
•	Validate with larger and more diverse datasets
•	Explore additional genres and demographics
•	Apply ensemble methods for stronger predictions
