# 🕵️ Fraud Detection using Machine Learning

Built ML models to detect fraudulent transactions with insights and prevention strategies.

## 📌 Project Overview  
This project focuses on detecting **fraudulent financial transactions** using machine learning models.  
The dataset contains over 6 million records, where fraud cases are **rare but highly impactful**.  

The goal is to:  
1. Clean and preprocess the dataset.  
2. Build and evaluate machine learning models for fraud detection.  
3. Identify key features contributing to fraud.  
4. Provide actionable recommendations to reduce fraudulent activity.  

---

## 📂 Dataset  
- **Source:** Provided by Accredian (CSV file with ~6.3M rows, 10 columns).  
- **Target Variable:** `isFraud` → 1 (fraud), 0 (genuine).  
- **Features:** Transaction details such as amount, type, and customer info.  

---

## ⚙️ Steps Performed  

### 1. Data Cleaning & Preparation  
- Removed duplicates and handled missing values.  
- Treated outliers by clipping extreme values.  
- Checked for multicollinearity among numeric features.  
- Splitted into **80% training** and **20% validation**.  

### 2. Model Building  
- **Logistic Regression** (with class balancing).  
- **Random Forest** (trained on a stratified sample for speed).  
- Compared models on metrics like **Precision, Recall, F1-score, ROC-AUC, PR-AUC**.  

### 3. Insights & Feature Importance  
- Top predictors of fraud include:  
  - **Transaction Amount** (large values linked to fraud).  
  - **Transaction Type/Merchant Category**.  
  - **Location/Device mismatch**.  
  - **Transaction frequency** (multiple rapid transactions).  

### 4. Business Recommendations  
- Add OTP/biometric for **high-value transactions**.  
- Implement **velocity checks** (block rapid multiple transactions).  
- Use **device/location fingerprinting** to flag unusual behavior.  
- Set **spending caps for new customers**.  
- Maintain **merchant risk scoring**.  

---

## 📊 Results  
- Logistic Regression: strong baseline performance.  
- Random Forest: better recall and interpretability through feature importance.  
- **Precision-Recall AUC** showed improvement over baseline models.  

---

## 🛠️ Tech Stack  
- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- **Tools:** Jupyter Notebook, GitHub  

---

## 📈 Future Work  
- Try advanced models (XGBoost, LightGBM, Neural Nets).  
- Deploy fraud detection model as a **real-time API**.  
- Implement **streaming analytics** for real-world use.  

---

## 📌 How to Run  
1. Clone this repository.  
2. Place dataset file (`fraud.csv`) in the project folder.  
3. Open the Jupyter Notebook:  
   ```bash
   jupyter notebook Accredian Fraud Detection.ipynb

## dataset 
link- https://drive.usercontent.google.com/download?id=1VNpyNkGxHdskfdTNRSjjyNa5qC9u0JyV&export=download&authuser=0
