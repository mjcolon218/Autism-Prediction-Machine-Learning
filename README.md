# 🧠 Autism Prediction using Machine Learning

This project builds a machine learning model to predict whether an individual is likely to be on the autism spectrum, based on a questionnaire and related features.

## 📁 Dataset
- Source: ASD Screening Dataset (`train.csv`)
- Features include:
  - Age, gender, country of residence
  - A1–A10 behavioral screening questions
  - Medical indicators: jaundice, autism history, app usage

---

## 🔍 Problem Statement

Build a binary classification model that:
- Predicts ASD likelihood from early screening data
- Maximizes **recall** (minimizes missed diagnoses)
- Balances **precision** (reduces false positives)

---

## 🧪 Models Tested

| Model                | Accuracy | Precision | Recall | F1 Score |
|----------------------|----------|-----------|--------|----------|
| Logistic Regression  | 84%      | 81%       | 87%    | 84%      |
| Support Vector Machine | 91%   | 84%       | 99%    | 91%      |
| XGBoost              | 95%      | 91%       | 100%   | 95%      |

✅ **XGBoost performed best** with perfect recall and high accuracy.

---

## ⚙️ Feature Engineering

- `sum_score`: Sum of A1–A10 behavioral scores
- `ind`: Combined indicator of jaundice, prior autism, app usage
- `age_log`: Log-transformed age
- `age_group`: Binned version of age

---

## 📊 Exploratory Data Analysis

- KDE and boxplots to visualize class differences
- Heatmaps to detect multicollinearity
- Distribution analysis to build intuition

---

## 📚 Lessons for Students

- Structured approach to ML classification tasks
- Data cleaning and feature preparation
- Understanding model behavior and trade-offs
- Logistic Regression as a solid baseline

---

## 🚀 How to Run

```bash
# 1. Clone the repo
git clone https://github.com/your-repo/autism-prediction.git

# 2. Launch Jupyter Notebook
jupyter notebook Autism_Prediction_Refactored_With_Models.ipynb

```

---

## ✨ Credits

- Created by **Maurice J. Colon**
- Educational use at **The Knowledge House**
