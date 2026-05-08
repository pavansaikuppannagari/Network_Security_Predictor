
# Network Anomaly Detection using Machine Learning

## 📌 Project Overview

This project builds a machine learning pipeline to detect **anomalous network load** based on traffic, resource, and security event features. The goal is to automatically flag unusual or potentially malicious network behavior (e.g., overload, attacks, misuse) so that security teams can take timely action.

The project uses the **Network Security Load Dataset** and focuses on **classical ML** (no heavy deep learning) with strong emphasis on:
- Imbalanced data handling
- Anomaly detection techniques
- Interpretable metrics for cybersecurity use cases

---

## 🧾 Problem Statement

Modern networks generate massive traffic logs, and it is no longer feasible for security analysts to manually inspect logs for anomalies. The problem is to:

> **Predict whether a given network state corresponds to normal or anomalous load using numerical and categorical features such as traffic metrics, system resource usage, and security events.**

This can support:
- Intrusion detection systems (IDS)
- Early warning for DDoS/overload
- Security monitoring dashboards

---

## 📂 Dataset

- **Source:** Kaggle – Network Security Load Dataset  
- **Link:** https://www.kaggle.com/datasets/ziya07/network-security-load-dataset  
- **Size:** 5,000+ rows, 22 columns  
- **Target:** `Anomalous_Load` (0 = Normal, 1 = Anomalous)

### Key Feature Groups

- **Traffic metrics:** packet size, transmission rate, active connections, latency  
- **System resources:** CPU usage, memory usage, bandwidth, response time  
- **Security events:** authentication failures, access violations, firewall blocks  
- **Signal features:** wavelet coefficients capturing temporal behavior  


## 🧪 Approach

### 1. Exploratory Data Analysis (EDA)
- Overview of class balance (normal vs anomalous)
- Summary statistics and correlation analysis
- Visualization of key features across normal/anomalous cases

### 2. Data Preprocessing
- Handle missing values (None)
- Feature scaling ( MinMaxScale)
- Train/validation/test split with stratification

### 3. Modeling

**Baseline model:**
- DecisionTreeClassifier

**Accurate model:**
- Gradient Boosting Classifier

### 4. Evaluation Metrics

The project focuses on:
- Precision, Recall, F1-score 
- ROC–AUC score
- Precision–Recall curve
- Confusion matrix interpretation from a security perspective

---

## 📊 Key Results

> Update this section after training:

- Best model: `GradientBoostingClassifier`  (to be finalized)
- F1-score (anomaly class): `01.00`
- Precision / Recall (anomaly class): `01.00 / 01.00`


---


