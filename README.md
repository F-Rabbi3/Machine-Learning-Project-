# 🚀 DDoS Attack Detection using Machine Learning & Deep Learning  
### CMP7239 – Applied Machine Learning Project

---

## 📌 Overview

This project focuses on detecting and classifying **DDoS attacks** using both **Machine Learning (ML)** and **Deep Learning (DL)** techniques on the **CIC-DDoS2019 dataset**.

The goal is to build a robust multi-class classification system that can accurately identify different types of DDoS attacks while handling **class imbalance** and improving **model generalisation**.

---

## 🧠 Key Highlights

- ✅ Multi-class DDoS attack classification  
- ✅ Combination of **ML + DL models**  
- ✅ Custom **Hybrid Loss Function (MSE + Cross-Entropy)**  
- ✅ Advanced preprocessing and feature engineering  
- ✅ Model optimisation with **GridSearchCV & class balancing**  
- ✅ Performance comparison across multiple models  

---

## 📂 Dataset

- **Dataset Name:** CIC-DDoS2019  
- **Source:** https://www.unb.ca/cic/datasets/ddos-2019.html  
- **Kaggle Link:** https://www.kaggle.com/datasets/dhoogla/cicddos2019  

### 📊 Dataset Details
- ~30GB raw data (sampled for training)
- 80+ network traffic features
- Multiple DDoS attack categories

---

## ⚙️ Technologies Used

- Python  
- NumPy, Pandas  
- Scikit-learn  
- XGBoost  
- TensorFlow / Keras  
- Matplotlib / Seaborn  

---

## 🔍 Project Workflow

1. **Data Loading & Sampling**
   - Large dataset handled using selective sampling

2. **Exploratory Data Analysis (EDA)**
   - Distribution analysis
   - Feature behaviour across attack types

3. **Data Preprocessing**
   - Handling missing values  
   - Feature scaling  
   - Encoding labels  

4. **Feature Importance Analysis**
   - Identify most relevant network traffic features  

5. **Model Training**
   - ML and DL models implemented  

6. **Model Evaluation**
   - Accuracy, Precision, Recall, F1-score, ROC-AUC  

---

## 🤖 Models Implemented

### 🔹 Machine Learning Models
- Random Forest  
- XGBoost  
- Decision Tree  
- K-Nearest Neighbours (KNN)  

### 🔹 Deep Learning Models
- Artificial Neural Network (ANN / MLP)  
- 1D Convolutional Neural Network (1D-CNN)  

---

## 💡 Innovation: Hybrid Loss Function

This project introduces a **custom hybrid loss function**:

- Combines:
  - Mean Squared Error (MSE)
  - Categorical Cross-Entropy (CE)

### 🎯 Why?

- Cross-Entropy → focuses on correct classification  
- MSE → improves probability calibration  

👉 Result: Better performance on **imbalanced multi-class data**

---

## 🛠️ Optimisation Techniques

### For ML Models
- GridSearchCV for hyperparameter tuning  
- Class weighting (`balanced`)  
- Oversampling to handle imbalance  

### For DL Models
- Hybrid Loss Function  
- Class-weighted training  
- Early stopping  
- Cosine learning rate scheduling  
- GlobalAveragePooling (CNN improvement)  

---

## 📈 Evaluation Metrics

Models are evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-Score  
- ROC-AUC  

---

## 📊 Results Summary

- **Random Forest & XGBoost** performed best among ML models  
- **CNN outperformed ANN** in deep learning models  
- Hybrid loss improved stability and generalisation  

---

## ▶️ How to Run

```bash
# Clone the repository
git clone https://github.com/your-username/your-repo-name.git

# Navigate to project folder
cd your-repo-name

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook cmp7239-2.ipynb
```

---

## 🎯 Use Cases

- Network intrusion detection systems (IDS)  
- SOC (Security Operations Center) automation  
- Real-time attack detection systems  
- Cybersecurity research  

---

## 🔮 Future Improvements

- Real-time deployment using streaming data  
- Integration with SIEM tools (Splunk, ELK)  
- Advanced DL models (LSTM, Transformer-based models)  
- Explainable AI (SHAP, LIME)  

---

## 📌 Conclusion

This project demonstrates how combining **Machine Learning and Deep Learning** with smart optimisation techniques can significantly improve **cyber attack detection systems**.

The introduction of a **Hybrid Loss Function** adds a unique contribution by improving model generalisation in complex, imbalanced datasets.
