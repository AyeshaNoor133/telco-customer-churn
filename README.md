# telco-customer-churn
# 📊 Customer Churn Prediction — Business Analysis

## 🎯 Task Summary
This project analyzes customer churn for a telecom company using **Logistic Regression** and a **Decision Tree Classifier** to identify key factors leading to customer loss and propose actionable business strategies.

---

## 📈 Model Comparison Table

| Model | Overall Accuracy | Precision (Churn) | Recall (Churn) | F1-Score (Churn) |
| :--- | :---: | :---: | :---: | :---: |
| **Logistic Regression** | ~0.74 | 0.51 | **0.80** | 0.62 |
| **Decision Tree (Depth=5)** | **0.76** | **0.54** | 0.71 | **0.61** |

> **Class Imbalance Note:** Only ~26.5% of customers churned in the dataset. Using `class_weight='balanced'` helped maintain high Recall scores, ensuring the model flags high-risk customers effectively.

---

## 🔑 Top 3 Drivers of Churn (Decision Tree)

1. **`Contract_Month-to-month` (60.9% Importance):** Customers on short-term month-to-month contracts are drastically more likely to leave.
2. **`OnlineSecurity_No` (10.7% Importance):** Lack of online security add-ons increases user friction and cancellation likelihood.
3. **`MonthlyCharges` (9.7% Importance):** Higher monthly bills directly correlates with a higher probability of churning.

---

## 💼 Business Summary (Executive Presentation)

Our analysis indicates that **contract structure is the single largest factor driving customer churn**, with month-to-month contracts accounting for over 60% of predictive importance. Customers paying high monthly fees without protective value-adds (like Online Security) show the highest risk of cancellation. To minimize churn, the business should incentivize customers to transition to 1- or 2-year contracts through targeted discounts, while bundling essential security add-ons into base subscription tiers to improve long-term retention.
