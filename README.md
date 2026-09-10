# 🛡️ ProbashiShield - AI-Powered Exploitative Clause Detection

ProbashiShield is a machine learning & deep learning pipeline to identify any exploitatively or unfairly written, or void clauses within the German employment contracts of Bangladeshi expatriates, through a dataset of 886 clauses categorized into three categories: valid (711), void (130), and unfair (45). Text preprocessing and feature extraction through TF-IDF (5,000 features, n-grams 1-2) for conventional methods and Keras tokenization for deep learning models have been done considering severe class imbalance with balanced class weights. Five models Dummy Classifier, Logistic Regression, Random Forest, XGBoost, and Bi-LSTM have been trained and tested where Logistic Regression proved the best with accuracy 81.95% and F1-Score 0.8081, which was also confirmed by 5-fold cross-validation results with mean F1-Score 0.8161. Evaluation metrics of the project include confusion matrices (showing the problem of classifying the minority "unfair" class), feature importance plots, and training curve of Bi-LSTM which shows overfitting from epoch 5, along with the architecture of the project in the output folder along with classification reports.
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
