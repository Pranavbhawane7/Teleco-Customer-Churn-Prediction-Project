## 📊 Telco Customer Churn Prediction

---

📌 Project Overview

Customer churn is a major challenge for telecommunication companies, as customer retention directly impacts business growth and profitability. This project develops a Machine Learning model to predict whether a customer is likely to churn based on customer demographics, account information, subscribed services, and billing details.

The goal is to help businesses identify at-risk customers and implement targeted retention strategies before customers leave the service.

---

🎯 Business Objective

The primary objectives of this project are:

Predict customer churn using historical customer data.
Identify the key factors influencing churn behavior.
Compare multiple Machine Learning algorithms.
Assist telecom companies in improving customer retention and reducing revenue loss.

---

📂 Dataset Information

The dataset contains information about telecom customers, including:

Customer demographic details
Account tenure
Service subscriptions
Internet services
Contract details
Billing information
Payment methods
Target Variable

Churn- Indicates whether a customer left the company (1) or remained (0)

---

🔍 Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand customer behavior and discover factors contributing to churn.

Analysis Performed
Churn distribution analysis
Contract type analysis
Monthly charges analysis
Tenure analysis
Payment method analysis
Internet service analysis
Service usage patterns

Key Insights

✅ Customers with month-to-month contracts showed higher churn rates.

✅ Customers with shorter tenure were more likely to leave.

✅ Higher monthly charges were associated with increased churn probability.

✅ Electronic check users demonstrated higher churn tendencies compared to other payment methods.

---
Some Observations - 
Churn and No Churn Distribution- 

<img width="781" height="580" alt="image" src="https://github.com/user-attachments/assets/79c09ca6-7722-4736-b3c9-aa743ea6f386" />

Tenure vs Churn

<img width="752" height="562" alt="image" src="https://github.com/user-attachments/assets/76b051f6-9858-444b-b2bc-d2eff98907ef" />

SHAP Analysis

<img width="767" height="741" alt="image" src="https://github.com/user-attachments/assets/630c65f8-6db7-432e-b3ca-628702649615" />

---

🛠 Data Preprocessing

Data Cleaning
Checked for missing values
Removed inconsistencies
Corrected data types where necessary
Feature Encoding
Binary categorical variables such as:

Yes → 1
No → 0
Nominal categorical variables were encoded using Label Encoding.

Feature Scaling
Numerical features were standardized using StandardScaler.

Train-Test Split
The dataset was split into training and testing datasets for model evaluation.

Handling Class Imbalance
SMOTE (Synthetic Minority Oversampling Technique) was applied to the training dataset to balance the target classes.

---

🤖 Machine Learning Models Used

Logistic Regression
- A baseline classification algorithm used to establish initial model performance.

Random Forest Classifier
- An ensemble learning algorithm that combines multiple decision trees to improve predictive accuracy.

XGBoost Classifier
- A gradient boosting algorithm capable of capturing complex relationships within customer data.

---

📈 Model Evaluation
Models were evaluated using the following performance metrics:

* Accuracy Score
* Precision
* Recall
* F1 Score
* ROC-AUC Score
* Confusion Matrix

---

🏆 Best Performing Model

After evaluating multiple Machine Learning algorithms, XGBoost achieved the highest predictive performance and was selected as the final model.

The model demonstrated strong capability in identifying customers likely to churn while maintaining a balanced trade-off between precision and recall.

⚙️ Machine Learning Workflow

Data Collection
        │
        ▼
Data Cleaning
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Feature Encoding
        │
        ▼
Train-Test Split
        │
        ▼
Feature Scaling
        │
        ▼
SMOTE
        │
        ▼
Model Training
(Logistic Regression,
 Random Forest,
 XGBoost)
        │
        ▼
Model Evaluation
        │
        ▼
Best Model Selection

---

🛠️ Technologies Used

* Programming Language
* Python
* Libraries
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Imbalanced-Learn (SMOTE)
* XGBoost
* SHAP
---

📁 Project Structure

Teleco-Customer-Churn-Prediction-Project/
│
├── Customer_Churn.ipynb
├── README.md
└── Dataset

---

🚀 Future Enhancements

* Hyperparameter tuning using GridSearchCV
* Feature importance analysis
* Model deployment using Streamlit
* Churn prediction web application
* Customer retention recommendation system
