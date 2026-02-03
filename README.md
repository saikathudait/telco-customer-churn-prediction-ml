# Predicting Customer Churn in the Telecom Sector Using Machine Learning

## Overview
Customer churn is a major challenge in the telecommunications industry, directly affecting revenue and long-term sustainability. This project uses machine learning techniques to predict whether a customer is likely to discontinue telecom services, enabling proactive and data-driven retention strategies.

The analysis is based on the Telco Customer Churn dataset and follows a complete predictive analytics workflow, including data preprocessing, exploratory data analysis, model development, and performance evaluation.

---

## Dataset
**Source:** Telco Customer Churn Dataset (Kaggle)  
**Records:** 7,043 customers  
**Features:** 21 variables  

The dataset includes:
- Customer demographics (gender, senior citizen status)
- Account information (tenure, contract type, payment method)
- Service usage (internet service, online security, tech support)
- Financial data (monthly charges, total charges)
- Target variable: Churn (Yes / No)

The dataset file included in this repository:
- `WA_Fn-UseC_-Telco-Customer-Churn.csv`

---

## Project Structure
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── telco-customer-churn-prediction-ml.ipynb
├── README.md


---

## Methodology
1. **Data Preparation**
   - Converted `TotalCharges` to numeric
   - Removed missing values
   - Encoded categorical variables using One-Hot Encoding
   - Standardised numerical features
   - Applied an 80/20 train-test split

2. **Exploratory Data Analysis**
   - Churn distribution analysis
   - Tenure and monthly charge behaviour
   - Correlation heatmap
   - Service-level churn insights

3. **Models Implemented**
   - Logistic Regression
   - Decision Tree Classifier
   - Random Forest Classifier (with GridSearchCV tuning)

4. **Evaluation Metrics**
   - Accuracy
   - Precision
   - Recall
   - F1 Score
   - ROC AUC
   - Confusion Matrix
   - ROC Curve

---

## Key Findings
- Logistic Regression achieved the best overall performance with strong generalisation.
- Random Forest captured non-linear patterns and provided feature importance insights.
- Decision Tree showed weaker performance due to overfitting.
- Tenure, MonthlyCharges, TotalCharges, contract type, and internet service were key churn drivers.

---

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## How to Run
1. Clone the repository
2. Install required libraries
3. Run the Python script:
```bash
python telco-customer-churn-prediction-ml.ipynb

