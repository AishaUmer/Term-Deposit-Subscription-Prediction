# Term-Deposit-Subscription-Prediction
This project predicts whether a bank customer will subscribe to a **term deposit** as a result of a marketing campaign. Using the **Bank Marketing Dataset (UCI Repository)**, we build machine learning models, evaluate their performance, and interpret predictions using SHAP.

---

## 🎯 Objective
- Predict customer subscription (`deposit = yes/no`)
- Understand key factors influencing subscription decisions
- Build interpretable machine learning models
- Provide actionable insights for marketing optimization

---

## 📂 Dataset Description
The dataset contains **17 features**, including:

- **Demographics:** age, job, marital status, education  
- **Financial attributes:** balance, loan, housing  
- **Campaign details:** contact type, duration, campaign count  
- **Previous interactions:** pdays, previous, poutcome  
- **Target:** `deposit` (yes/no)

Source: UCI Machine Learning Repository – Bank Marketing Dataset

---

## 🧠 Approach

### 1️⃣ Data Loading & Exploration
- Loaded dataset using pandas  
- Performed EDA: distributions, correlations, class imbalance  

### 2️⃣ Preprocessing
- One‑Hot Encoding for categorical variables  
- Train-test split (80/20)  
- Target encoded as binary (yes=1, no=0)

### 3️⃣ Model Training
Two models were trained:
- **Logistic Regression**
- **Random Forest Classifier**

### 4️⃣ Evaluation Metrics
- Confusion Matrix  
- F1‑Score  
- ROC Curve & AUC  

### 5️⃣ Explainability
- Used **SHAP** to interpret model predictions  
- Explained **5 individual predictions**  
- Generated SHAP summary plots

---

## 📊 Results & Findings

### ✔ Random Forest performed best overall  
- Higher F1‑Score  
- Better ROC‑AUC  
- More robust to nonlinear relationships  

### ✔ Key Predictive Features
- **duration** (most influential)
- **poutcome**
- **balance**
- **age**
- **contact type**

### ✔ Insights
- Longer calls strongly correlate with subscription  
- Customers with successful past outcomes are more likely to subscribe  
- Repeated contact attempts reduce conversion probability  
- Cellular contact is more effective than telephone  

---

## 📝 Conclusion
The model effectively predicts customer subscription behavior and provides interpretable insights using SHAP. These insights can help banks:

- Optimize marketing campaigns  
- Reduce unnecessary outreach  
- Improve customer targeting  
- Increase term deposit conversions  

---

## 📁 Files Included
- `bank_marketing_model.py` – Full ML pipeline  
- `README.md` – Project documentation  
- `data/bank.csv`



