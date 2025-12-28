# Diabetes Regression using Linear & Random Forest Regression

This project demonstrates a **regression problem** where the goal is to predict a **continuous disease progression score** using machine learning models and evaluate how close the predictions are to the actual values.

---

## 📊 Dataset

- **Dataset**: Diabetes dataset from `sklearn`
- **Problem Type**: Regression
- **Target Variable**: `target` (numeric disease progression score)
- **Features**: Medical measurements such as BMI, blood pressure, etc.
- Dataset is small, clean, and suitable for learning regression fundamentals.

---

## 🎯 Problem Statement

Predict the disease progression score based on multiple medical features and evaluate the model performance using regression metrics.

---

## 🤖 Models Used

### 1️⃣ Linear Regression (Baseline Model)
- Assumes a **linear relationship** between features and target
- Used as a **baseline** model
- Requires **feature scaling**
- Simple and interpretable

### 2️⃣ Random Forest Regressor
- Ensemble model using **multiple decision trees**
- Captures **non-linear relationships**
- Does **not require feature scaling**
- Final prediction is the **average of predictions from all trees**

---

## 🔄 Approach

1. Load and explore the dataset  
2. Separate features (`X`) and target (`y`)  
3. Split data into training (80%) and testing (20%) sets  
4. Train models:
   - Linear Regression (with StandardScaler)
   - Random Forest Regressor (without scaling)
5. Evaluate models on unseen test data  

---

## 📏 Evaluation Metrics

Since this is a **regression problem**, the following metrics are used:

- **MSE (Mean Squared Error)** – Average squared prediction error  
- **RMSE (Root Mean Squared Error)** – Average prediction error in original units  
- **R² Score** – Proportion of variance in the target explained by the model  

---

## 📈 Results

| Model | RMSE | R² |
|------|------|----|
| Linear Regression | ~53.85 | ~0.45 |
| Random Forest Regressor | ~54.69 | ~0.49 |

---

## 🧠 Key Learnings

- Regression predicts **continuous numeric values**, not classes  
- Predictions are **approximate**, not exact  
- **RMSE** tells how wrong the model is on average  
- **R²** shows how well the model explains data variation  
- More complex models do **not always significantly reduce prediction error**, even if they capture patterns better  

---

## ✅ Conclusion

Random Forest Regressor slightly improves the **R² score**, indicating better capture of non-linear relationships, while the **RMSE remains similar** to Linear Regression. This shows that increased model complexity does not always lead to large improvements in prediction accuracy.

---

## 🚀 Future Improvements

- Hyperparameter tuning for Random Forest  
- Feature importance analysis  
- Trying Gradient Boosting models  

---

## 📌 Tech Stack

- Python  
- pandas  
- NumPy  
- scikit-learn  
