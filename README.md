# Customer Churn Prediction 🔮

A machine learning project to predict customer churn for a telecom company using the IBM Telco Customer Churn dataset.

## 📊 Project Overview
Customer churn prediction helps businesses identify customers likely to leave so they can take proactive retention steps. This project builds and compares multiple ML models to predict churn with high accuracy.

## 🗂️ Dataset
- **Source:** IBM Telco Customer Churn (Kaggle)
- **Size:** 7,032 rows × 19 features
- **Target:** Churn (Yes = 1 / No = 0)

## 🛠️ Tech Stack
- Python, Pandas, NumPy
- Scikit-learn, XGBoost
- Imbalanced-learn (SMOTE)
- Matplotlib, Seaborn

## ⚙️ Steps Performed
1. Data Loading & Exploration
2. Data Cleaning (TotalCharges fix, null handling)
3. Exploratory Data Analysis (EDA)
4. Feature Encoding & Scaling
5. Handling Class Imbalance with SMOTE
6. Model Building (Logistic Regression, Random Forest, XGBoost)
7. Evaluation (Accuracy, ROC-AUC, Confusion Matrix)
8. Hyperparameter Tuning (RandomizedSearchCV)
9. Feature Importance Analysis
10. Business Insights & Recommendations

## 📈 Model Results

| Model               | Accuracy | ROC-AUC |
|---------------------|----------|---------|
| Logistic Regression | 73.63%   | 83.34%  |
| Random Forest       | 77.19%   | 81.16%  |
| XGBoost             | 77.11%   | 81.79%  |
| XGBoost (Tuned)     | 77.40%   | 81.62%  |

**Best Model: Logistic Regression (ROC-AUC: 83.34%)**

## 🔍 Key Findings
- Month-to-month contract customers churn the most (~42%)
- New customers (tenure < 12 months) are at highest risk
- Fiber optic internet users churn more than DSL users
- High monthly charges correlate strongly with churn

## 💡 Business Recommendations
- Offer loyalty discounts to month-to-month customers
- Create onboarding programs for first 12 months
- Bundle security & tech support with fiber plans
- Review fiber optic pricing strategy
