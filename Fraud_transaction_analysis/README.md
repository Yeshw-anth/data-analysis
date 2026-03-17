# 💳 Hybrid Fraud Detection System

## 🚀 Overview
This project builds a **hybrid fraud detection system** to identify suspicious financial transactions using:

- 📊 Statistical method: **Z-score (user-level)**
- 🤖 Machine Learning: **Isolation Forest**

The system combines both approaches to detect **behavioral anomalies** in transaction data, simulating a real-world fraud detection pipeline.

---

## 🎯 Objective
Detect anomalous transactions **without labeled data** by leveraging:
- User-specific statistical deviations
- Multivariate anomaly detection

---

## 🧠 Approach

### 🔹 Feature Engineering
- Transaction-to-balance ratio  
- Online vs offline transaction indicator  
- Debit/Credit flag  
- High-risk age group flag  

---

### 🔹 Statistical Detection
- Applied **Z-score per user**
- Identifies transactions deviating from individual behavior

---

### 🔹 Machine Learning Model
- Used **Isolation Forest**
- Detects anomalies based on multiple features

---

### 🔹 Hybrid Scoring
- Final Score = 0.4 × Z-score Flag + 0.6 × ML Flag
- Combines statistical and behavioral signals
- Improves robustness over single-method approaches

---

## ⏳ Real-World Simulation
- Data sorted chronologically  
- Model trained on past transactions  
- Predictions made on future data  

👉 Mimics real-world fraud detection deployment

---

## 📊 Key Results

- 🚨 **~2% (1.98%) transactions flagged as anomalous**
- 💰 Anomalies linked to:
  - Higher transaction amounts  
  - High transaction-to-balance ratios  
- 🔐 Suspicious patterns include:
  - Increased login attempts  
  - Longer transaction durations  
- 🌐 Online transactions show higher anomaly rates

---

## 📊 Visual Insights

### Fraud Rate Over Time
![Fraud Trend](images/fraud_trend.png)

---

### Transaction Amount Distribution
![Distribution](images/distribution.png)

---

### Fraud vs Normal Comparison
![Boxplot](images/amount_boxplot.png)

---

## 💰 Business Impact:
- Early fraud detection reduces financial loss
- Hybrid approach reduces false positives
- System can be adapted for real-time monitoring

---

## 🛠️ Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn (Isolation Forest)  
- SciPy (Z-score)  
- Matplotlib, Seaborn  

---

## ⚠️ Limitations

- No labeled fraud data → cannot compute accuracy/recall  
- Isolation Forest depends on contamination assumption  
- Z-score assumes statistical distribution  

---

## 🚀 Future Improvements

- Use labeled dataset with supervised models (XGBoost, Random Forest)  
- Deploy real-time fraud detection API  
- Add model monitoring & drift detection  

---

## 📂 Project Files
fraud-detection/
│
├── fraud_detection.ipynb
├── README.md
├── requirements.txt

---

## 🏆 Key Takeaways

- Built a **hybrid anomaly detection system**
- Simulated **real-world deployment using time-based split**
- Combined **statistical + ML techniques**
- Focused on **behavioral insights and interpretability**

---

## 📬 Contact
Feel free to connect if you'd like to discuss or improve this project!
