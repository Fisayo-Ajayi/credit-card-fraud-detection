# Credit Card Fraud Detection using Machine Learning

## 1. Business Context

Fraud detection is a critical problem in financial systems, where fraudulent transactions are rare but highly impactful. Detecting these cases requires models that can handle extreme class imbalance.

---

## 2. Objective

To build a machine learning model capable of accurately identifying fraudulent transactions while minimizing missed fraud cases.

---

## 3. Dataset

- Original dataset: ~144,000 transactions  
- Sampled dataset: ~14,000 transactions  
- Fraud rate: ~0.19% (highly imbalanced)

---

## 4. Key Challenges

- Severe class imbalance (fraud cases are extremely rare)  
- High cost of false negatives (missed fraud)  
- Need for robust evaluation beyond accuracy  

---

## 5. Approach

- Data preprocessing:
  - Feature scaling (Time, Amount)
  - Outlier handling (winsorization)
- Class imbalance handling:
  - Applied class weighting in model training
- Model:
  - Random Forest Classifier

---

## 6. Model Performance

- Recall (fraud): ~86%  
- Precision (fraud): ~75%  
- ROC-AUC: ~0.9996  

The model demonstrates strong ability to detect fraudulent transactions while maintaining high overall performance.

---

## 7. Key Insight

Optimizing for recall is critical in fraud detection, as missing fraudulent transactions carries a higher cost than false positives.

---

## 8. Limitations

- Fraud cases are limited in the sampled dataset  
- Performance should be validated on larger, real-world datasets  

---

## 9. Project Assets

- 📄 Report: `reports/fraud-detection-analysis.pdf`  
- 📓 Notebook: `notebooks/fraud_detection.ipynb`  

---

## 10. Tools

- Python (Pandas, NumPy)
- Scikit-learn
- Seaborn, Matplotlib