# 🏦 Loan Default Risk Prediction (Banking Sector)

This project analyzes a large-scale banking dataset to predict the risk of loan default using statistical and machine learning models. It demonstrates data preprocessing, exploratory data analysis (EDA), feature engineering, and model evaluation — all presented in a clean, reproducible Jupyter Notebook.

---

## 📁 Dataset Overview

The dataset contains over 250,000 loan records with features like:

- **Demographics**: Age, Education, Marital Status
- **Financials**: Income, LoanAmount, Credit Score, Interest Rate
- **Loan Details**: Purpose, Term, DTI Ratio, Mortgage, Co-Signer
- **Target**: `Default` (0 = No, 1 = Yes)

---

## 🧠 Key Tasks Performed

- ✅ Data loading, inspection, and cleaning
- 📊 Descriptive statistics and correlation heatmap
- 📉 Visualizations: loan purpose, education, default distribution
- 🧹 Feature engineering: binary encoding, one-hot encoding
- 🔍 Statistical modeling using **Logistic Regression**
- 📈 Machine learning using **K-Nearest Neighbors (KNN)**
- 🧪 Evaluation using Accuracy, Precision, Recall, F1-score, ROC-AUC
- 💾 Saved visuals in `/Visuals/` folder

---

## 🧪 Models Built

| Model                | Accuracy | Recall (Default) | AUC Score |
|---------------------|----------|------------------|-----------|
| Logistic Regression | 88.6%    | 3%               | ✅        |
| K-Nearest Neighbors | 87.5%    | 5%               | ✅        |

> Class imbalance remains a challenge — future work could include SMOTE or cost-sensitive models.

---

## 📂 Folder Structure

Hospital_Readmission_Risk_Prediction/
├── readmission_analysis.ipynb
├── visuals/
│ ├── correlation_heatmap.png
│ ├── confusion_matrix.png
│ ├── roc_curve_logreg.png
│ ├── confusion_matrix_knn.png
│ └── roc_curve_knn.png
├── data/
│ └── loan_data.csv
└── README.md



---

## ⚙️ Tools & Libraries Used

- Python, Pandas, NumPy
- Matplotlib, Seaborn
- scikit-learn
- statsmodels

---

## 📌 Future Enhancements

- Implement Random Forest and XGBoost
- Apply resampling methods (e.g., SMOTE)
- Deploy using Streamlit for real-time risk prediction

---

## 📬 Contact

Created by **Milan Suthar**  
🌐 [LinkedIn](https://www.linkedin.com/in/milan-kumar-suthar-3b95b0281)

---

