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
## 🚀 How It Works

1. Load and clean server log data  
2. Convert categorical log fields into numeric features  
3. Apply Isolation Forest  
4. Get anomaly scores for each log entry  
5. Filter out entries above anomaly threshold  
6. Visualize anomaly patterns  

---

## 📈 Visualizations

The notebook includes:

- Traffic pattern plots  
- Anomaly score distribution  
- Highlighted anomalous requests  
- Time-series anomaly visualization  

---

## ✅ Results

The model successfully:

- Identified abnormal traffic spikes  
- Detected suspicious IP behavior  
- Found rare access patterns not present in normal logs  

---

## 📌 Future Improvements

- Use LSTM models for time-series predictions  
- Integrate with real-time log monitoring  
- Deploy using FastAPI or Flask  
- Add dashboard visualization using Streamlit  

---

## 🧑‍💻 Author  
**Hitesh Duggal**  
B.Tech CSE | Data Science & ML Enthusiast

