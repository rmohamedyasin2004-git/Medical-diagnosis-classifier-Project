# Medical-Diagnosis-classifier-project
# 🩺 Clinical Diagnostic Classification Pipeline using Stratified Cross-Validation

## 📋 Project Overview
This project implements an end-to-end binary classification pipeline designed to differentiate between malignant and benign tumors using the Wisconsin Breast Cancer diagnostic dataset. Built with production-ready machine learning best practices, the system emphasizes high medical recall to minimize false-negative predictions, ensuring critical clinical cases are accurately detected.

## ⚙️ Technical Architecture & Workflow
- **Data Preprocessing & Imputation:** Handled missing values using median imputation and standardized numerical features via `StandardScaler` to optimize gradient convergence.
- **Robust Validation Strategy:** Implemented **5-Fold Stratified Cross-Validation** to preserve class distribution proportions across folds and prevent data leakage.
- **Model Exploration & Benchmarking:** Evaluated multiple supervised algorithms including Logistic Regression, Decision Trees, and Random Forest classifiers.
- **Class-Imbalance Handling:** Applied balanced class-weighting parameters to penalize misclassifications of minority classes.

## 📈 Performance & Evaluation Metrics
Evaluated across multiple out-of-fold metrics to ensure clinical reliability:
- **ROC-AUC Score:** Achieved an exceptional mean ROC-AUC of **0.9951 ± 0.0055**, demonstrating superior separability between classes.
- **Recall / Sensitivity:** Maintained a robust mean recall of **95.77%**, ensuring minimal risk of missed malignant diagnoses (False Negatives).
- **Out-of-Fold Accuracy & Precision:** Reached **97.19%** accuracy and **96.67%** precision, balancing false positives and patient anxiety.

## 📊 Visual Outputs & Interpretability
- **Confusion Matrix:** Visualized out-of-fold true/false positive and negative distributions.
- **ROC Curve:** Plotted true positive rate against false positive rate across probability thresholds.
- **Feature Importance:** Extracted top clinical indicators (such as worst perimeter, area, and concave points) using Gini impurity rankings from tree-based models.

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib

## 💡 Clinical & Ethical Considerations
In medical machine learning, metrics like **Recall** take precedence over raw accuracy. Failing to detect a malignant case (False Negative) carries severe clinical risks compared to a False Positive, which leads to secondary screening. This pipeline is tuned to balance threshold probabilities responsibly.
