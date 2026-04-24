# 🏥 Patient Disease Prediction
### ML Lab — Midterm Project

![Python](https://img.shields.io/badge/Python-3.x-blue) ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange) ![Colab](https://img.shields.io/badge/Google-Colab-yellow)

---

## 📌 Project Overview
This project predicts whether a patient has a disease based on their health data using **Supervised Machine Learning (Binary Classification)**.

A custom dataset of **500 patient records** was generated with real-world inspired health features.

---

## 📂 Dataset Details
| Feature | Description |
|---------|-------------|
| Age | Patient age (20–80 years) |
| BloodPressure | Blood pressure in mmHg |
| BloodSugar | Blood sugar level in mg/dL |
| BMI | Body Mass Index |
| Cholesterol | Cholesterol level in mg/dL |
| HeartRate | Heart rate (beats per minute) |
| Smoking | Smoking status (0 = No, 1 = Yes) |
| Disease | Target variable (0 = Healthy, 1 = Disease) |

- **Total Records:** 500  
- **Healthy Patients:** 182 (36.4%)  
- **Disease Patients:** 318 (63.6%)  

---

## 🔍 Exploratory Data Analysis (EDA)
- Dataset info, shape, and data types
- Statistical summary (mean, std, min, max)
- Missing values check → ✅ No missing values
- Class distribution (Bar + Pie chart)
- Feature distributions (Histograms)
- Correlation Heatmap
- Boxplots by Disease Status

---

## 🤖 Algorithms Used

### 1️⃣ Logistic Regression
- Linear classification algorithm
- Uses sigmoid function to predict probability
- Feature scaling applied (StandardScaler)

### 2️⃣ Random Forest Classifier
- Ensemble of 100 decision trees
- Captures non-linear patterns
- No scaling required
- Provides feature importance scores

---

## 📊 Results Comparison

| Metric | Logistic Regression | Random Forest |
|--------|-------------------|---------------|
| Accuracy | 81.00% | **83.00%** ✅ |
| Precision | 84.62% | 84.06% |
| Recall | 85.94% | **90.62%** ✅ |
| F1 Score | 85.27% | **87.22%** ✅ |
| AUC Score | 0.912 | **0.920** ✅ |

### 🏆 Best Model: Random Forest
Random Forest outperforms Logistic Regression across all major metrics especially **Recall (90.62%)** which is critical in medical diagnosis.

---

## 🔑 Feature Importance (Random Forest)
| Rank | Feature | Importance |
|------|---------|------------|
| 1 | BloodSugar | 24.5% |
| 2 | Age | 17.8% |
| 3 | BloodPressure | 16.7% |
| 4 | Smoking | 12.7% |
| 5 | BMI | 10.4% |
| 6 | Cholesterol | 10.2% |
| 7 | HeartRate | 7.7% |

---

## 🛠️ Tools & Libraries
- **Language:** Python 3.x
- **Platform:** Google Colab
- **Libraries:** NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn

---

## 👨‍💻 Author
**Adrash Bhatia**  
ML Lab — Midterm Project
