# server-log-anomaly-detection
# 🚨 Server Log Anomaly Detection using Isolation Forest

This project detects anomalies in server logs using **Isolation Forest**, an unsupervised machine learning algorithm widely used for outlier detection. The goal is to identify unusual patterns in log data that may indicate **potential security threats, unauthorized access, or abnormal system behavior**.

---

## 📂 Project Overview

Modern servers generate large volumes of log data, making manual monitoring difficult.  
This project automates anomaly detection by:

- Preprocessing raw log files
- Extracting meaningful features (IP hits, timestamps, request patterns, etc.)
- Training an Isolation Forest model
- Identifying unusual or suspicious log entries
- Visualizing anomaly distribution

This approach performs significantly better than clustering-based methods like K-Means for detecting rare anomalies.

---

## 🧠 Machine Learning Used

### **Isolation Forest**
- Specifically designed for anomaly detection  
- Performs well on imbalanced datasets  
- Identifies points that are easier to isolate  
- Handles high-dimensional data efficiently  

---

## 📊 Features Extracted
- Request timestamps  
- IP address frequency  
- URL endpoints accessed  
- Request methods (GET/POST)  
- Time-based traffic patterns  
- Status codes  

---

## 🛠 Tech Stack

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib / Seaborn**
- **Scikit-learn**
- **Jupyter Notebook**

---

## 📁 Project Structure

