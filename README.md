# 💳 Credit Card Fraud Detection

A machine learning project that detects fraudulent credit card transactions using **Decision Tree** and **Random Forest** classifiers.

---

##  Project Overview

Credit card fraud is a growing financial threat worldwide. This project builds a supervised machine learning pipeline to classify transactions as **genuine** or **fraudulent** using anonymised PCA features from real-world transaction data.

---

##  Dataset

- **Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Total Transactions:** 2,84,807
- **Features:** 28 PCA components (V1–V28) + Amount + Time
- **Target:** Class (Genuine, Fraud)

| Class | Count | Percentage |
|-------|-------|------------|
| Genuine | 2,84,315 | 99.8273% |
| Fraud | 492 | 0.1727% |

---

##  Technologies Used

- Python 3
- Pandas & NumPy
- Matplotlib
- Scikit-learn

---

##  Project Workflow

1. **Load Dataset** – Load and explore the CSV file
2. **Null Value Check** – Verify no missing values exist
3. **Transaction Analysis** – Count genuine vs fraud transactions
4. **Visualization** – Bar graph of class distribution
5. **Normalization** – StandardScaler applied to Amount column
6. **Train/Test Split** – 70:30 ratio
7. **Model Training** – Decision Tree & Random Forest
8. **Predictions** – predict() on test set
9. **Accuracy Comparison** – score() for both models
10. **Performance Matrix** – Confusion matrix, Precision, Recall, F1-Score

---

##  Results

### Model Accuracy

| Model | Accuracy |
|-------|----------|
| **Decision Tree** | 99.9293% |
| **Random Forest** | **99.9532%** |

### Performance Metrics

| Metric | Decision Tree | Random Forest |
|--------|:---:|:---:|
| Precision | 13.333% | **57.143%** |
| Recall | 11.765% | **23.529%** |
| F1-Score | 12.500% | **33.333%** |

### Confusion Matrix

| | Predicted Genuine | Predicted Fraud |
|---|:---:|:---:|
| **Actual Genuine** (DT) | 85269 | 26 |
| **Actual Fraud** (DT) | 39 | 109 |
| **Actual Genuine** (RF) | 85290 | 5 |
| **Actual Fraud** (RF) | 35 | 113 |

---

##  Conclusion

**Random Forest outperforms Decision Tree** across all metrics:
- Higher accuracy (99.95% vs 99.92%)
- Much better precision (57.1% vs 13.3%)
- Better recall (23.5% vs 11.8%)
- Better F1-Score (33.3% vs 12.5%)

Random Forest is the preferred model for fraud detection as it correctly identifies more fraud cases while generating fewer false positives.

---

## 📁 Files

```
📦 Credit-Card-Fraud-Detection
 ┣ 📓 Credit_Card_Fraud_Detection.ipynb   # Main notebook
 ┣ 📄 README.md                           # Project documentation
 ┗ 📄 creditcard.csv                      # Dataset (download from Kaggle)
```

## 👤 Author

**Aryaman Vishnoi**  
📧 bishnoiarav24@gamil.com  
🔗 [LinkedIn](https://www.linkedin.com/in/aryamanvishnoi-data/) | [GitHub](https://github.com/aryaman-data)
