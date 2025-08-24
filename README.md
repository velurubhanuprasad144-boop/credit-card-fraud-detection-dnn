# Credit Card Fraud Detection using Deep Neural Networks

## 📌 Project Overview
This project implements a **Deep Neural Network (DNN)** to detect fraudulent credit card transactions.  
The goal is to build a reliable machine learning model that can distinguish between **fraudulent** and **legitimate** transactions in highly imbalanced datasets.

---

## 📊 Dataset
- **Source**: [Credit Card Fraud Detection Dataset (Kaggle)](https://www.kaggle.com/mlg-ulb/creditcardfraud)  
- **Details**:  
  - 284,807 transactions  
  - 492 fraud cases (highly imbalanced)  
  - Features are anonymized (PCA transformed) except `Time` and `Amount`  
  - Target: `Class` → `0` (legitimate) or `1` (fraudulent)

---

## ⚙️ Methodology
1. **Data Preprocessing**  
   - Normalization of `Amount` and `Time`  
   - Handling class imbalance using techniques such as **SMOTE** or **undersampling**  

2. **Model Architecture (DNN)**  
   - Input layer: (number of features)  
   - Hidden layers: Dense layers with ReLU activation + Dropout  
   - Output layer: Sigmoid activation (binary classification)  

3. **Training**  
   - Loss function: Binary Crossentropy  
   - Optimizer: Adam  
   - Evaluation metrics: Accuracy, Precision, Recall, F1-score, AUC  

---

## 🏆 Results
| Metric       | Value (example) |
|--------------|-----------------|
| Accuracy     | 99.2%           |
| Precision    | 92.5%           |
| Recall       | 84.1%           |
| F1-score     | 88.1%           |
| AUC-ROC      | 0.98            |

📌 *Update this table with your actual results.*  
📈 Add confusion matrix, ROC curve, and precision-recall plots as images here.

---

## 🚀 How to Run
### 1. Clone the Repository
```bash
git clone https://github.com/your-username/credit-card-fraud-detection-dnn.git
cd credit-card-fraud-detection-dnn
