# Obesity Risk Prediction Project
This project applies machine learning techniques to predict the likelihood of an individual developing obesity based on demographic, lifestyle, and dietary factors. By leveraging a dataset of 1,610 individuals from Türkiye, the project aims to support healthcare professionals in identifying high-risk individuals and formulating targeted interventions to mitigate obesity-related health issues.

# Project Background
Obesity has become a significant public health challenge globally, contributing to chronic conditions like diabetes, cardiovascular diseases, and certain cancers. Traditional healthcare approaches have struggled to address obesity’s multifactorial nature. By incorporating machine learning, this project aims to identify obesity risks more effectively and provide data-driven solutions for prevention and intervention.

# Objectives
- Develop machine learning models to predict obesity risk using demographic, lifestyle, and dietary features.
- Compare the performance of various predictive models to identify the most effective approach.
- Provide actionable insights for healthcare professionals to improve prevention strategies.

# Dataset
The dataset, sourced from Kaggle (Koklu & Sulak, 2024), consists of data on 1,610 individuals, including:
- Demographic Factors: Age, Sex, Height, etc.
- Lifestyle Factors: Physical Exercise, Type of Transportation Used, etc.
- Dietary Habits: Frequency of Fast Food Consumption, Number of Main Meals Daily, etc.
- Target Variable: Weight classification (Underweight, Normal, Overweight, Obesity).
Link: https://www.kaggle.com/datasets/suleymansulak/obesity-dataset

# Methodology
1. Data Cleaning:
- Verified no missing values.
- Detected and addressed outliers in key features (e.g., Age, Height).

2. Exploratory Data Analysis (EDA):
- Visualized distributions and relationships using pie charts, bar charts, and histograms.
-Identified trends linking features to obesity risk.

3. Data Preprocessing:
- Applied log transformation to reduce skewness in Age.
- Performed label encoding for binary features.

4. Class Imbalance Handling:
- Addressed class imbalance using SMOTE (Synthetic Minority Over-sampling Technique).

5. Model Development:
Utilized StratifiedKFold for cross-validation.
Trained and evaluated models including Random Forest, achieving 88% accuracy.

6. Deployment:
Exported the trained Random Forest model using pickle.
Deployed a Flask web application for real-time predictions.

# Results
- The Random Forest Classifier achieved the highest accuracy of 88%.
- Key predictive features include Age, Physical Exercise, Height, Frequency of Consuming Vegetables, and Number of Main Meals Daily.
- Visualizations of feature importance and their relationships with weight class highlighted actionable insights for intervention strategies.

# Deployment
The model has been deployed via a Flask web application that allows users to input their data and receive obesity risk predictions in real-time. This tool aims to provide early warnings and encourage proactive lifestyle changes.

# Contributors
Tan Rik Ee, Teo Kai Ning, Tan Jian Lin, Yuki Sim Tze Yii, Chua Sze Yan, Low Zi Yang

This project is a step toward leveraging data-driven insights for addressing the obesity epidemic. Contributions and feedback are welcome to improve the approach and its applicability.
