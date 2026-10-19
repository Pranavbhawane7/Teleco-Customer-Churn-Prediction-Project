### 📊 Telco Customer Churn Prediction

---

📌 Project Overview
Customer churn is one of the most critical challenges faced by telecommunication companies. Losing existing customers directly impacts revenue and increases customer acquisition costs.

This project aims to predict whether a customer is likely to churn using Machine Learning techniques and identify the key factors that influence customer attrition.

The project follows an end-to-end Data Science workflow including data preprocessing, feature engineering, handling class imbalance, model training, evaluation, and model explainability using SHAP.

---

🎯 Business Objective
The primary objective of this project is to:

Predict customers who are likely to leave the company.
Identify important churn-driving factors.
Enable proactive customer retention strategies.
Support data-driven business decisions.

---


📂 Dataset Information
Dataset: Telco Customer Churn Dataset

Features include:
Customer demographics
Account information
Contract details
Internet services
Billing information
Additional service subscriptions
Target Variable
Variable	Description
Churn	0 = Customer Retained, 1 = Customer Churned
🛠️ Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-Learn
XGBoost
SHAP
Imbalanced-Learn (SMOTE)

---

🔄 Project Workflow
Data Collection
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
Feature Engineering
      ↓
Encoding Categorical Variables
      ↓
Train-Test Split
      ↓
Feature Scaling (StandardScaler)
      ↓
SMOTE for Class Balancing
      ↓
Model Training
      ↓
Model Evaluation
      ↓
SHAP Explainability
      ↓
Business Insights

---

🧹 Data Preprocessing
Several preprocessing steps were performed:

Data Cleaning
Checked missing values
Converted data types where necessary
Handled inconsistent values
Encoding
Binary categorical variables were converted into numerical values:

Original	Encoded
Yes	1
No	0
Feature Scaling
Numerical features were standardized using:

StandardScaler()
Scaled features:

Tenure
MonthlyCharges
TotalCharges

---

⚖️ Handling Class Imbalance
The dataset exhibited class imbalance between churn and non-churn customers.

To address this issue:

SMOTE()
was applied on the training dataset to generate synthetic samples for the minority class.

Benefits:

Improved model learning
Reduced class bias
Better churn detection performance
🤖 Machine Learning Models
The following classification models were trained and evaluated:

1. Logistic Regression
Baseline model
Easy to interpret
Fast training
2. Random Forest
Ensemble learning method
Handles non-linear relationships
Provides feature importance
3. XGBoost
Gradient boosting algorithm
High predictive performance
Effective handling of complex patterns

---

📈 Model Evaluation Metrics
The models were evaluated using:

Accuracy
Precision
Recall
F1-Score
ROC-AUC Score
Confusion Matrix

---

🏆 Final Model
XGBoost
XGBoost was selected as the final model due to its superior predictive performance and robustness.

Advantages:

✅ Better generalization

✅ Handles non-linearity effectively

✅ Strong predictive capability

✅ Performs well on imbalanced datasets

---

🔍 Model Explainability with SHAP
To improve model transparency and interpretability, SHAP (SHapley Additive Explanations) was used.

Purpose of SHAP
Explain model predictions
Identify influential features
Improve stakeholder trust
Generate actionable business insights
Key Features Influencing Churn
Contract Type
Tenure
Monthly Charges
Online Security
Tech Support
Total Charges

---

💡 Business Insights
Key observations from the analysis:

Customers with Month-to-Month contracts show higher churn rates.
Customers with shorter tenure are more likely to leave.
Higher monthly charges contribute to churn.
Lack of Online Security increases churn probability.
Lack of Tech Support is associated with higher customer attrition.
🚀 Business Recommendations
Customer Retention Strategies
Encourage customers to switch to longer-term contracts.
Improve onboarding experience for new customers.
Offer retention incentives to high-risk customers.
Promote Online Security and Tech Support services.
Deploy predictive models within CRM systems for proactive retention campaigns.
📷 Project Visualizations
The project includes:

Exploratory Data Analysis (EDA)
Class Distribution Analysis
Correlation Analysis
Model Evaluation Metrics
Confusion Matrix
ROC Curve
SHAP Summary Plot
Feature Importance Analysis

---

📁 Repository Structure
├── Customer_Churn.ipynb
├── README.md
├── images/
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   ├── shap_summary_plot.png
│   └── feature_importance.png
🎯 Future Improvements
Hyperparameter Optimization
Model Deployment using Flask/FastAPI
Real-Time Churn Prediction
Customer Retention Recommendation Engine
Interactive Dashboard Development
](https://github.com/Pranavbhawane7/Teleco-Customer-Churn-Prediction-Project/blob/main/Customer_Churn.ipynb)
