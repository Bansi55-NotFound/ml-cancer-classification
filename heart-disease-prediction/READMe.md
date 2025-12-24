# Heart Disease Prediction using Logistic Regression

This project builds an end-to-end machine learning model to predict whether a patient has heart disease using medical attributes.  
It focuses on correct model evaluation and interpretation of metrics for a healthcare use case.

---

## Problem Statement
Predict whether a patient has **heart disease (1)** or **no heart disease (0)** based on clinical and demographic features.

This is a **binary classification** problem where missing a disease case is more critical than raising a false alarm.

---

## Dataset
The dataset contains medical features such as:
- Age
- Sex
- Chest pain type
- Resting blood pressure
- Cholesterol
- Maximum heart rate
- Exercise-induced angina
- ST depression and slope
- Number of major vessels
- Thalassemia

**Target column:**
- `1` → Heart disease present  
- `0` → No heart disease

---

## Approach
1. Data loading and inspection  
2. Separation of features (X) and target (y)  
3. Train/Test split (80/20)  
4. Feature scaling using `StandardScaler`  
5. Model training using **Logistic Regression**  
6. Model evaluation using:
   - Confusion Matrix
   - Accuracy
   - Precision
   - Recall
   - ROC–AUC

---

## Evaluation Results
- **Accuracy:** ~85%
- **Precision:** ~87%
- **Recall:** ~84%
- **ROC–AUC:** ~0.93

### Interpretation
- The model shows **good overall performance**
- Some heart disease cases are missed, indicating scope for improvement
- Strong ROC–AUC score indicates good class separation

---

## Tools &
