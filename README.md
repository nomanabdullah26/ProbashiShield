# ProbashiShield

# 🛡️ ProbashiShield - AI-Powered Exploitative Clause Detection

বাংলাদেশি প্রবাসী কর্মীদের জার্মান কর্মসংস্থান চুক্তিতে শোষণমূলক ধারা সনাক্তকরণের জন্য মেশিন লার্নিং ও ডিপ লার্নিং মডেল।

---

## 📊 ডেটাসেট ওভারভিউ

মোট ক্লজ: **886টি**  
লেবেল: **valid**, **unfair**, **void**

![লেবেল ডিস্ট্রিবিউশন](outputs/label_distribution.png)

---

## 🤖 মডেল পারফরম্যান্স তুলনা

| মডেল | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Dummy (Baseline) | 0.8045 | 0.6472 | 0.8045 | 0.7174 |
| Logistic Regression | **0.8195** | **0.8001** | **0.8195** | **0.8081** |
| Random Forest | 0.8195 | 0.8039 | 0.8195 | 0.7617 |
| XGBoost | 0.8195 | 0.8080 | 0.8195 | 0.7717 |
| Bi-LSTM | 0.8120 | 0.7950 | 0.8120 | 0.7346 |

🏆 **সেরা মডেল:** Logistic Regression (F1-Score: 0.8081)

![মডেল তুলনা](outputs/model_comparison.png)

---

## 📈 কনফিউশন ম্যাট্রিক্স (Logistic Regression)

![কনফিউশন ম্যাট্রিক্স](outputs/confusion_matrix.png)

---

## 🔍 গুরুত্বপূর্ণ ফিচার (Random Forest)

![ফিচার ইমপোর্ট্যান্স](outputs/feature_importance.png)

---

## 📉 Bi-LSTM ট্রেনিং কার্ভ

![Bi-LSTM ট্রেনিং কার্ভ](outputs/bilstm_training_curves.png)

---

## 📋 ক্লাসিফিকেশন রিপোর্ট (Logistic Regression)
