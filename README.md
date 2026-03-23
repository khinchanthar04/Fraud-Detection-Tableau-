# Credit Card Fraud Detection Analysis

**Khin Chan Thar**

---

## 📌 Overview

This project presents an exploratory data analysis of credit card fraud patterns, using transaction-level data to identify key risk signals and evaluate the effectiveness of existing fraud prevention mechanisms. The analysis spans transaction volume, amount distribution, chargeback behaviour, foreign transaction exposure, and currency-level fraud rates by culminating in targeted recommendations to improve detection accuracy.

---

## 🔎 Key Areas of Analysis

### 1. 📊 Overall Transaction Patterns
Baseline profiling of transaction volume and amount distribution across all records, establishing the foundation for fraud-specific comparisons.

### 2. 🕵 Fraud Detection Dashboard
Breakdown of total records by fraud status and foreign transaction status. A key finding: **fraudulent transactions are disproportionately represented among cross-border payments**, highlighting foreign transactions as a primary vulnerability.

### 3. 🔄 Transaction Amount & Daily Chargeback
Scatter plot analysis reveals a **clear positive relationship** between transaction amount and average daily chargeback. This effect is amplified in fraudulent transactions where high-value payments carry significantly greater financial risk and require tighter monitoring.

### 4. 🔢 Average Amount by Fraud Status
Fraudulent transactions consistently involve **higher average amounts** compared to legitimate ones, reinforcing the value of amount-based thresholds in fraud detection systems.

### 💲 5. Fraud by Currency
Currency-level analysis shows that **fraud rates vary significantly across regions**, with certain currencies exhibiting elevated incidence. This points to targeted vulnerabilities in cross-border payment channels.

### 6. 🦺 Safety Net Effectiveness
Evaluation of current fraud prevention mechanisms reveals critical gaps:
- The number of transaction **declines does not increase significantly with transaction amount**, meaning high-value and therefore riskier transactions are not being flagged at a higher rate.
- Roughly half of legitimate transactions per day experience declines, generating **false positives** and unnecessary customer friction.
- The overall finding: the safety net reduces friction but is **not catching enough fraud**, leaving clear room for algorithm improvement.

---

## 📋 Findings Summary

| Signal | Insight |
|---|---|
| Foreign transactions | Disproportionately higher fraud rate |
| Transaction amount | Higher amounts correlate with higher fraud and chargebacks |
| Currency | Fraud rates vary significantly by currency/region |
| Decline behaviour | Weak correlation with transaction amount — high-value fraud is under-flagged |
| False positives | High for legitimate transactions — detection needs re-tuning |

---

## ✍️ Recommendations

1. **Strengthen cross-border payment rules** — implement stricter checks for foreign transactions, especially in currencies with the highest fraud incidence.
2. **Amount-based thresholds** — adjust fraud detection sensitivity for high-value transactions, which correlate strongly with chargebacks.
3. **Currency-level risk rules** — tailor fraud detection logic by currency and require additional verification for transactions in high-risk regions.
4. **Behavioural and pattern profiling** — apply customer-level behavioural analysis to detect anomalies that rule-based systems miss.
5. **Reduce false positives** — re-calibrate detection algorithms to reduce unnecessary friction for legitimate customers while improving fraud capture rates.

---

## Project Structure

```
├── 14684190_KhinChan_Fraud_Detection.pptx   # Full presentation and dashboards
├── 14684190_KhinChan_Fraud_Detection.twbx   # Tableau file
├── creditcard_fraud_detection.csv           # Full presentation and dashboards
└── README.md                                # This file

```

---

## Author

**Khin Chan Thar**  
Credit Card Fraud Detection — Data Analysis Project
