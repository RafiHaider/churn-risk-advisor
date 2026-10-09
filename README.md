# 📉 Customer Churn Risk Advisor

An interactive decision-support application built with **Streamlit** and **XGBoost** to predict customer churn probability, assign risk bands, and provide prescriptive retention strategies for telco operators.

---

## 🚀 Live Application & Repository
* **Live Web App:** [Customer Churn Risk Advisor on Streamlit Cloud](https://churn-risk-advisor-td2kkqsa9zbfrf8scabsbk.streamlit.app/) 
* **GitHub Repository:** [RafiHaider/churn-risk-advisor](https://github.com/RafiHaider/churn-risk-advisor)

---

## 📌 Project Overview & Features

The **Churn Risk Advisor** bridges the gap between raw machine learning output and real-world business intervention. Key capabilities include:

* **Real-time Individual Scoring:** Input specific customer attributes via a sidebar form to instantaneously generate a churn probability score, assigned risk band (LOW / MEDIUM / HIGH), and recommended outreach action.
* **Prescriptive Counterfactual Analysis:** Dynamic *"What would change the risk?"* feature computes probability deltas for potential contract and service upgrades.
* **Batch Scoring & Export:** Drag and drop CSV customer data to process batch predictions, highlight high-risk accounts above a customizable threshold, and export scored reports.
* **Explainable AI (XAI):** Feature contribution breakdowns showing key factors driving risk up or down.

---

## 📊 Model Performance & Specification

* **Algorithm:** `XGBClassifier`
* **Validation Performance:** Cross-Validation AUC of **$0.845 \pm 0.012$**
* **Feature Schema:** 19 customer attributes including tenure, contract type, payment method, internet services, and billing preferences.

---

## 📁 Repository Structure

```text
churn-risk-advisor/
├── app.py                   # Streamlit web application interface
├── churn_model.joblib       # Trained XGBoost classification model binary
├── model_meta.json          # Model metadata, feature list, and performance metrics
├── requirements.txt         # Pinned Python dependencies for cloud execution
├── sample_customers.csv     # Sample batch dataset for testing
└── README.md                # Project documentation
