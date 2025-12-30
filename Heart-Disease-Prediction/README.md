---

# ❤️ Heart Disease Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.9-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![Healthcare](https://img.shields.io/badge/Domain-Healthcare-red)

---

## 📌 Project Overview

Cardiovascular diseases (CVDs) are the **leading cause of death worldwide**, accounting for nearly **31% of global deaths**.
Early detection of heart disease can significantly reduce mortality through preventive care and timely intervention.

This project aims to:

* Analyze patient health data
* Build machine learning models to **predict heart disease**
* Provide **actionable recommendations** to hospitals for prevention

---

## 🎯 Problem Statement

### Task 1

Prepare a **complete data analysis report** on the given dataset.

### Task 2

Build **machine learning models** to predict potential heart diseases.

### Task 3

Provide **suggestions to hospitals** to prevent life-threatening situations using predictions.

---

## 🏥 Domain

**Healthcare / Medical Analytics**

---

## 📂 Dataset Information

* Source: Public Heart Disease Dataset
* Format: CSV
* Total Records: ~300+ patients
* Features: 13 input features + 1 target variable

### Target Variable

| Value | Meaning               |
| ----- | --------------------- |
| 0     | No heart disease      |
| 1     | Heart disease present |

---

## 🧾 Feature Description

| Feature                              | Description            |
| ------------------------------------ | ---------------------- |
| age                                  | Age of patient         |
| sex                                  | 0 = Female, 1 = Male   |
| chest_pain_type                      | Chest pain category    |
| resting_blood_pressure               | Resting BP             |
| serum_cholesterol_mg_per_dl          | Cholesterol level      |
| fasting_blood_sugar_gt_120_mg_per_dl | Diabetes indicator     |
| resting_ekg_results                  | ECG results            |
| max_heart_rate_achieved              | Max heart rate         |
| exercise_induced_angina              | Exercise chest pain    |
| oldpeak_eq_st_depression             | ST depression          |
| slope_of_peak_exercise_st_segment    | ST slope               |
| num_major_vessels                    | Blocked vessels        |
| thal                                 | Thallium stress test   |
| target                               | Heart disease (output) |

---

## ⚙️ Technologies Used

* **Python**
* **Pandas, NumPy**
* **Matplotlib, Seaborn**
* **Scikit-Learn**
* **XGBoost**
* **Jupyter Notebook**

---

## 🔍 Exploratory Data Analysis (EDA)

Key observations:

* Risk increases significantly after age 45
* Males show higher heart disease prevalence
* Chest pain type and blocked vessels are strong predictors
* Lower max heart rate correlates with heart disease

---

## 🧠 Machine Learning Models

The following models were trained and evaluated:

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Decision Tree
* Random Forest
* **XGBoost (Best Model)** ✅

---

## 📊 Model Performance Comparison

| Model               | Accuracy | ROC-AUC  |
| ------------------- | -------- | -------- |
| Logistic Regression | ~85%     | 0.88     |
| KNN                 | ~82%     | 0.84     |
| Decision Tree       | ~79%     | 0.81     |
| Random Forest       | ~88%     | 0.91     |
| **XGBoost**         | **~90%** | **0.93** |

### 🏆 Best Model: **XGBoost**

* Highest accuracy and ROC-AUC
* Handles non-linear patterns well
* Suitable for production deployment

---

## 🔑 Important Features (XGBoost)

Top contributors:

* Number of major vessels
* Chest pain type
* ST depression (oldpeak)
* Maximum heart rate
* Thallium stress test result

---

## ⚠️ Challenges Faced & Solutions

| Challenge        | Solution                    |
| ---------------- | --------------------------- |
| Mixed data types | One-Hot Encoding            |
| Feature scaling  | StandardScaler              |
| Overfitting      | Ensemble models             |
| Interpretability | Feature importance analysis |
| Class imbalance  | ROC-AUC as main metric      |

---

## 🏥 Hospital Recommendations

1. **Early Screening**

   * Integrate ML model into OPD systems
   * Flag high-risk patients automatically

2. **Preventive Care**

   * Regular ECG & cholesterol checks
   * Lifestyle counseling for high-risk individuals

3. **Focused Monitoring**

   * Male patients aged 45+
   * Patients with blocked vessels or high ST depression

4. **Model Retraining**

   * Update model every 6–12 months with new data

---

## 📁 Project Structure

```
Heart-Disease-Prediction/
│
├── Heart_Disease_Prediction.ipynb
├── README.md
├── dataset/
│   └── heart.csv
└── images/
```

---

## 🚀 How to Run

1. Clone the repository

```bash
git clone https://github.com/your-username/HeartDiseasePrediction.git
```

2. Open Jupyter Notebook

```bash
jupyter notebook
```

3. Run `Heart_Disease_Prediction.ipynb`

---

## ✅ Conclusion

This project demonstrates how **machine learning can assist healthcare professionals** in early detection of heart disease, enabling preventive action and saving lives.

---

## 👤 Author

**Kishore Das**
