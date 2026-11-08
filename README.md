# Medical-diagnosis-classifier-Project

# 🩺 Medical Diagnosis Classifier with Cross-Validation

An end-to-end machine learning classification pipeline built to diagnose malignant vs. benign medical cases using robust validation techniques.

## 🚀 Key Highlights & Performance
- **Dataset:** Breast Cancer Wisconsin Dataset (569 samples, 30 features)
- **Validation Strategy:** 5-Fold Stratified Cross-Validation to prevent data leakage and handle class distribution fairly.
- **Best Model:** Logistic Regression (Optimized via Pipeline with Imputation and Standard Scaling)
- **Evaluation Metrics:**
  - **Mean ROC-AUC:** 0.9951 ± 0.0055
  - **Mean Recall (Sensitivity):** 95.77% (Critical for minimizing false negatives in medical diagnostics)
  - **Out-of-Fold Accuracy:** 97.19%

## 📊 Visualizations & Outputs
- **Confusion Matrix:** Out-of-fold classification breakdown.
- **ROC Curve:** High true-positive vs false-positive rate separation.
- **Feature Importance:** Top clinical indicators ranked via Random Forest feature importances.

## 🛠️ Tech Stack
- Python, Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib

## 📝 Clinical & Ethical Considerations
In medical machine learning, high **Recall** is prioritized to ensure critical positive cases are not missed, while maintaining balanced precision to prevent unnecessary patient anxiety.
