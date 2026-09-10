# 🛡️ ProbashiShield - AI-Powered Exploitative Clause Detection

Machine Learning and Deep Learning models for detecting exploitative clauses in German employment contracts for Bangladeshi expatriate workers.

---

## 📊 Dataset Overview

Total Clauses: **886**  
Labels: **valid**, **unfair**, **void**

<p align="center">
  <img src="label_distribution.png" alt="Label Distribution" width="800">
</p>

---

## 🤖 Model Performance Comparison

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Dummy (Baseline) | 0.8045 | 0.6472 | 0.8045 | 0.7174 |
| Logistic Regression | **0.8195** | **0.8001** | **0.8195** | **0.8081** |
| Random Forest | 0.8195 | 0.8039 | 0.8195 | 0.7617 |
| XGBoost | 0.8195 | 0.8080 | 0.8195 | 0.7717 |
| Bi-LSTM | 0.8120 | 0.7950 | 0.8120 | 0.7346 |

🏆 **Best Model:** Logistic Regression (F1-Score: 0.8081)

<p align="center">
  <img src="model_comparison.png" alt="Model Comparison" width="800">
</p>

---

## 📈 Confusion Matrix (Logistic Regression)

<p align="center">
  <img src="confusion_matrix.png" alt="Confusion Matrix" width="700">
</p>

---

## 🔍 Important Features (Random Forest)

<p align="center">
  <img src="feature_importance.png" alt="Feature Importance" width="700">
</p>

---

## 📉 Bi-LSTM Training Curves

<p align="center">
  <img src="bilstm_training_curves.png" alt="Bi-LSTM Training Curves" width="900">
</p>

---

## 📋 Classification Report (Logistic Regression)

*(Note: You can add your specific classification report metrics for Logistic Regression here)*

---

## 🏗️ Framework Architecture

<p align="center">
  <img src="Screenshot 2026-07-14 112337.png" alt="ProbashiShield Framework Architecture" width="900">
</p>

---

## 📁 Project Structure

```text
ProbashiShield/
│
├── data/                   # Dataset files
├── models/                 # Saved trained models
├── outputs/                # Generated plots and reports
│   ├── label_distribution.png
│   ├── model_comparison.png
│   ├── confusion_matrix.png
│   ├── feature_importance.png
│   ├── bilstm_training_curves.png
│   └── Screenshot 2026-07-14 112337.png
├── src/                    # Source code for training and evaluation
└── README.md               # Project documentation
