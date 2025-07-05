# 🧬 Cervical Cancer Risk Prediction using Machine Learning

This project builds a machine learning pipeline to **predict the likelihood of cervical cancer** based on behavioral, demographic, and medical history data. The goal is to enable early screening support and raise awareness about risk factors—particularly in low-resource settings where diagnosis is often delayed.

---

## 📁 Dataset Summary
**Samples**: 858  
**Features**: 36 (demographics, STDs, contraceptive use, habits, etc.)  
**Target Variable**: `Biopsy` (1 = positive for cervical cancer, 0 = negative)

---

## 📌 Project Highlights

- 🔍 Cleaned and preprocessed messy medical data with missing values encoded as `"?"`
- 📊 Performed thorough Exploratory Data Analysis (EDA)
- 🧠 Trained and evaluated classification models (XGBoost, etc.)
- 🎯 Achieved high accuracy while mitigating overfitting via cross-validation

---

## 🧪 Features (Columns)

A few key columns from the dataset:

- `Age`
- `Number of sexual partners`
- `First sexual intercourse`
- `Num of pregnancies`
- `Smokes`, `Smokes (years)`, `Smokes (packs/year)`
- `Hormonal Contraceptives`, `IUD`
- Multiple `STDs:*` columns
- `Dx:Cancer`, `Dx:HPV`, `Dx:CIN`
- Target tests: `Hinselmann`, `Schiller`, `Citology`, and **`Biopsy`** ✅

---

## 🔧 Preprocessing

- Replaced `"?"` with `NaN`
- Converted all applicable columns to numeric
- Imputed missing values using:
  - Median for numerical features
  - Mode for binary categorical variables
- Removed high-missing-value features (if above 60%)
- Standardized numerical features

---

## 🛠️ Tech Stack

- Python 3.x
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
---
