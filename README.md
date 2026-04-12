# 💳 Loan Default Risk Prediction using Machine Learning

## 📌 Project Overview

Loan defaults create significant financial risk for banks and lending institutions by increasing losses, reducing portfolio quality, and impacting profitability. Predicting potential defaulters before loan approval helps organizations make smarter lending decisions and improve risk management.

This project uses a real-world **Loan Default Dataset** to analyze borrower profiles and predict whether a customer is likely to default on a loan using machine learning classification models.

The workflow includes **data cleaning, missing value treatment, outlier handling, exploratory data analysis, leakage detection, model building, evaluation, and business recommendations**.

---

## 🎯 Objectives

✔ Analyze borrower data to identify key default risk factors
✔ Clean and preprocess financial data for modeling
✔ Detect and remove target leakage variables
✔ Build and compare multiple machine learning models
✔ Evaluate models using business-relevant metrics
✔ Generate insights to support credit approval decisions

---

## 📊 Dataset Information

* **Dataset Name:** Loan Default Dataset
* **Records:** 148,670 loan applications
* **Features:** 34 original variables
* **Final Features Used:** 18 predictors after cleaning
* **Target Variable:** `Status`

### Example Features:

* Loan Amount
* Income
* Credit Score
* Loan Type
* Loan Purpose
* Property Value
* Loan-to-Value (LTV)
* Debt-to-Income Ratio (DTI)
* Age
* Region

---

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Libraries:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn
* **Environment:** Jupyter Notebook

---

## ⚙️ Project Workflow

### 1️⃣ Data Preprocessing

✔ Removed irrelevant columns (`ID`, constant fields)
✔ Handled missing values using median/mode imputation
✔ Treated outliers using IQR capping
✔ Encoded categorical variables using one-hot encoding
✔ Applied feature scaling where required

### 2️⃣ Leakage Detection & Correction ⭐

Initial models showed unrealistic perfect accuracy. A detailed leakage audit was performed, and post-decision proxy variables were removed to ensure trustworthy model performance.

### 3️⃣ Exploratory Data Analysis

✔ Loan default distribution
✔ Credit score vs default
✔ Income vs default
✔ Loan amount vs default
✔ Borrower segment analysis
✔ Correlation heatmap

### 4️⃣ Models Implemented

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier
* K-Nearest Neighbors (KNN)
* Naive Bayes

---

## 📈 Final Model Performance

| Model               | Accuracy   | ROC-AUC   |
| ------------------- | ---------- | --------- |
| Logistic Regression | 77.46%     | 0.689     |
| Decision Tree       | 82.10%     | 0.769     |
| **Random Forest**   | **89.18%** | **0.878** |
| KNN                 | 79.79%     | 0.747     |
| Naive Bayes         | 74.48%     | 0.680     |

### 🏆 Best Model: Random Forest

* **Accuracy:** 89.18%
* **Precision:** 93.16%
* **Recall:** 60.55%
* **F1 Score:** 73.39%
* **ROC-AUC:** 0.878

---

## 🔍 Key Insights

🔹 Credit Score was a major predictor of loan default risk.
🔹 Higher LTV and weaker borrower financial profiles increased default probability.
🔹 Random Forest captured nonlinear risk patterns better than linear models.
🔹 Leakage removal significantly improved project reliability and realism.

---

## 💡 Business Recommendations

✔ Use predictive scoring during loan approval screening
✔ Review high-risk applications manually
✔ Apply stricter checks for weak credit profiles
✔ Optimize lending portfolio using risk segmentation
✔ Continuously retrain model with new applicant data

---

## 📁 Project Structure

```bash id="j4p7zn"
loan_default_prediction/
│── Loan_Default.csv
│── loan_default_model.ipynb
│── best_loan_default_model.pkl
│── loan_model_comparison.csv
│── README.md
```

---

## 🚀 Future Improvements

* Hyperparameter tuning
* SMOTE for class imbalance
* XGBoost / LightGBM implementation
* Streamlit loan risk dashboard
* Explainable AI (SHAP values)

---

## 👨‍💻 Author

**Milan Kumar Suthar**
M.Sc. Statistics & Computing, BHU
Aspiring Data Analyst | Machine Learning Enthusiast

---

## ⭐ If you found this project useful, feel free to star the repository.
