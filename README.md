# 🔐 Server Log Anomaly Detection for Cybersecurity  
Using Unsupervised Machine Learning (Isolation Forest, DBSCAN, KMeans, One-Class SVM)

This project applies multiple unsupervised machine learning techniques to detect anomalies in server logs and network traffic. It was developed as part of the **NIELIT Summer Training Programme in Data Science Using Python (2025)**.

The goal is to identify suspicious activities, unusual traffic behavior, and potential cyberattacks using clustering and anomaly detection models.

---

## 📌 Project Overview

Modern cybersecurity threats are increasingly sophisticated, making traditional signature-based intrusion detection insufficient.  
This project uses **unsupervised learning** to detect unknown and zero-day threats by analyzing network traffic patterns without requiring labeled data.

You implemented and compared four models:

- **Isolation Forest** (best performance)
- **K-Means Clustering**
- **DBSCAN**
- **One-Class SVM**

The dataset contains **40,000 synthetic network events** with features like IP addresses, ports, protocol, packet length, severity, and traffic types.

---

## 🚀 Objectives

- Identify anomalies in server logs and network traffic  
- Compare unsupervised ML models for intrusion detection  
- Perform feature engineering and dimensionality reduction  
- Analyze model outputs and visualize anomalies  
- Evaluate how well these methods detect potential cyberattacks  

---

## 🧠 Machine Learning Models Used

### **1. Isolation Forest (Recommended)**
- Best anomaly detection performance  
- Identified 3–5% suspicious events  
- Handles high-dimensional and imbalanced data well  

### **2. K-Means Clustering**
- Weak performance for anomalies  
- Helpful for general traffic grouping  
- High DBI and low Silhouette Score  

### **3. DBSCAN**
- Good at identifying dense vs sparse regions  
- Highly sensitive to `eps` and `min_samples`  

### **4. One-Class SVM**
- Conservative anomaly detection  
- Best for detecting subtle boundary anomalies  

---

## 🔧 Tech Stack

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib / Seaborn**
- **Jupyter Notebook**

---

## 📊 How It Works

1. Load and inspect server log / network traffic dataset  
2. Clean and preprocess data (handle missing values, encode categories)  
3. Perform feature engineering (timestamp features, frequency encoding, IP hashing)  
4. Scale numerical features  
5. Apply dimensionality reduction (PCA, t-SNE for visualization)  
6. Train anomaly detection models (Isolation Forest, DBSCAN, etc.)  
7. Calculate anomaly scores and detect suspicious events  
8. Visualize clustering and anomaly patterns  
9. Compare all models using metrics & visual analysis  

---

---

## 📈 Results & Discussion

- **Isolation Forest** produced the most meaningful and interpretable anomalies.  
- **DBSCAN** detected a large number of noise points but was highly sensitive to parameters.  
- **K-Means** failed to isolate outliers due to overlapping cluster shapes.  
- **One-Class SVM** was accurate but flagged fewer anomalies.  
- Visualizations (t-SNE, PCA) helped confirm anomaly separations.  

---

## 🛡 Key Insights

- Unsupervised learning can detect threats without needing labeled attack data.  
- Feature engineering significantly improves anomaly separation.  
- Isolation Forest + PCA gives the best practical results.  
- Synthetic datasets are useful for modeling but need real-world validation.  

---

## 🔮 Future Improvements

- Apply deep learning models for sequence-based logs  
- Deploy a real-time monitoring pipeline with alerts  
- Integrate with a dashboard (Streamlit / Grafana)  
- Test on real server logs for better accuracy  

---

## 👨‍💻 Author

**Hitesh Duggal**  
B.Tech CSE | Data Science & Machine Learning Enthusiast  
NIELIT Summer Training – Data Science Using Python (2025)



