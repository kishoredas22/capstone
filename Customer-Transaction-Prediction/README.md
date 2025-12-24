# 📊 Customer Transaction Prediction (Banking Domain)

## 📌 Project Overview

This project focuses on predicting whether a customer will make a transaction in the future using anonymized banking data.
The solution helps banks improve **targeted marketing**, **customer engagement**, and **revenue optimization**.

The project is implemented as a **single, end-to-end Jupyter Notebook**, covering data analysis, model building, comparison, and final recommendations.

---

## 🎯 Problem Statement

Banks want to identify customers who are likely to make a transaction in the future, irrespective of the transaction amount.

### Objective

Build a machine learning model that predicts:

* **1** → Customer will make a transaction
* **0** → Customer will not make a transaction

---

## 🏦 Domain

**Banking / Finance**

---

## 📂 Dataset Description

* The dataset is **anonymized**
* Total records: **200,000**
* Total features: **202**

  * `ID_code` → Unique customer identifier
  * `var_0` to `var_199` → Anonymized numerical features
  * `target` → Binary target variable

⚠️ Since feature names are anonymized, traditional exploratory data analysis (EDA) is limited.

---

## 🧠 Machine Learning Task

* **Type:** Supervised Learning
* **Problem:** Binary Classification

---

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Libraries:**

  * NumPy, Pandas
  * Scikit-learn
  * XGBoost
  * Matplotlib, Seaborn
* **Environment:** Jupyter Notebook (Anaconda)

---

## 📘 Project Workflow

1. Problem understanding & dataset overview
2. Data integrity checks (missing values, duplicates, variance)
3. Data preprocessing

   * ID column removal
   * Stratified train–test split
   * Feature scaling
4. Model building

   * Logistic Regression (baseline)
   * Random Forest
   * XGBoost
5. Model evaluation using ROC-AUC
6. Model comparison & final recommendation
7. Challenges faced & solutions
8. Final conclusion

---

## 📊 Evaluation Metric

Due to strong class imbalance (~90:10), **ROC-AUC** was chosen as the primary evaluation metric.

Additional metrics:

* Precision
* Recall
* F1-Score
* Confusion Matrix

---

## 🤖 Models Used

### 1️⃣ Logistic Regression

* Baseline model
* Simple and interpretable
* Provides a benchmark

### 2️⃣ Random Forest

* Captures non-linear relationships
* Improves recall
* Shows overfitting tendencies

### 3️⃣ XGBoost ✅ (Final Model)

* Best performance on test data
* Highest ROC-AUC
* Better generalization
* Industry-standard for tabular banking data

---

## 🏆 Model Comparison Summary

| Model               | Test ROC-AUC | Recall (Class 1) |
| ------------------- | ------------ | ---------------- |
| Logistic Regression | ~0.85        | ~0.30            |
| Random Forest       | ~0.89        | ~0.40            |
| **XGBoost**         | **~0.91**    | **~0.45–0.50**   |

📌 **XGBoost is recommended for production use.**

---

## ⚠️ Challenges Faced & Solutions

| Challenge           | Solution             | Reason                           |
| ------------------- | -------------------- | -------------------------------- |
| Anonymized features | Model-based learning | Feature semantics unavailable    |
| Class imbalance     | ROC-AUC metric       | Robust to imbalance              |
| High dimensionality | Tree-based models    | Capture feature interactions     |
| Overfitting         | Gradient boosting    | Better generalization            |
| Scaling requirement | StandardScaler       | Required for Logistic Regression |

---

## ✅ Final Conclusion

The project successfully delivers a robust customer transaction prediction system using anonymized banking data.
Among all evaluated models, **XGBoost** achieved the best performance and is recommended for real-world deployment.

---

## 🔮 Future Improvements

* Threshold optimization
* Model explainability using SHAP
* API deployment (FastAPI)
* Monitoring & retraining pipeline

---

## 📁 Repository Structure

```
Customer-Transaction-Prediction/
│
├── Customer_Transaction_Prediction.ipynb
├── train.csv
└── README.md
```

---

## 📌 How to Run

1. Clone the repository
2. Place `train.csv` in the same directory as the notebook
3. Open `Customer_Transaction_Prediction.ipynb`
4. Run cells from top to bottom

---

## 👤 Author

**Kishore**

