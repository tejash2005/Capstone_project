# Capstone_project
Customer Purchase Prediction using Machine Learning

1. Introduction

This project aims to develop a predictive model that determines whether a customer will make a purchase based on demographic and behavioral attributes. Using a structured ML pipeline, the project performs extensive data preprocessing, exploratory data analysis (EDA), feature transformation, and model evaluation to identify the best-performing classifier for purchase prediction.

The dataset includes features such as: CURR_AGE, GENDER, ANN_INCOME, AGE_CAR, PURCHASE (Target variable)

2. Data Preprocessing
The workflow includes all essential preprocessing steps required for a robust classification model:

2.1 Dataset Cleaning
Removal of duplicates
Handling of missing values
Standardizing/normalizing numerical columns
Encoding categorical variables (LabelEncoder for GENDER)

2.2 Feature Engineering & Transformation
Correlation analysis using heatmaps
Outlier inspection through boxplots
Distribution assessment using histograms
Scaling of numerical variables using StandardScaler

3. Exploratory Data Analysis (EDA)
The notebook contains multiple EDA visualizations:
Countplot for PURCHASE distribution
Countplot for GENDER separation
Distribution plots for ANN_INCOME, AGE_CAR, and CURR_AGE
Correlation heatmap to understand feature relationships

Key observations include:
Clear imbalance between purchase and non-purchase classes
Purchase behavior shows a correlation with age and income variables

4. Model Development

The project explores multiple machine-learning algorithms:

4.1 Models Trained
Logistic Regression
Decision Tree Classifier
Random Forest Classifier
XGBoost Classifier (used with tuned hyperparameters)

4.2 Train-test Split

Dataset split into X_train, X_test, y_train, y_test (80–20)

4.3 Evaluation Metrics Used
Accuracy
Precision
Recall
F1-score

Confusion Matrix

The notebook also prints Classification Reports for each model.

5. Results & Performance
Based on the evaluation metrics printed in your notebook (classification reports), the following conclusions can be drawn:
Logistic Regression: Stable baseline performance but limited non-linearity capture
Decision Tree: High variance and risk of overfitting
Random Forest: Stronger generalization, improved accuracy
XGBoost: Best performance overall, offering high predictive power and optimal precision–recall balance
XGBoost emerged as the top-performing model in the project.

Although the notebook shows metric outputs, the summary interpretation is:
✔ High classification accuracy
✔ High precision in predicting purchasers
✔ Lower misclassification compared to other models

6. Benefits of the Project
This machine-learning implementation provides multiple practical benefits:
Business Benefits
Accurate prediction of potential buyers
Improved targeting and personalized marketing
Enhanced customer segmentation
Reduction in campaign waste and improved ROI

Technical Benefits:
Modular ML pipeline
Scalable preprocessing and modeling workflow
Easily integrable with dashboards and APIs
Supports future enhancements like deep learning or real-time prediction

7. Conclusion
The project successfully implements a structured machine-learning pipeline to predict customer purchase decisions. Through extensive preprocessing, EDA, and comparative model evaluation, XGBoost is identified as the most effective classifier. This model can significantly assist businesses in understanding customer behavior and optimizing marketing strategies.

The project lays a strong foundation for future expansion, including:
Feature enrichment with behavioral data
Real-time predictive systems
Integration with recommendation engines
Deployment using dashboards or cloud services
