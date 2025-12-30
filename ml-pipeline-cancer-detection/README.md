# End-to-End Machine Learning Pipeline — Cancer Detection

This project demonstrates a complete **end-to-end machine learning pipeline** built using scikit-learn.  
It covers the full ML lifecycle from data loading to model saving, following practices used in real-world ML systems.

---

## 🎯 Objective

To build a **production-style ML pipeline** that:
- Trains a classification model
- Evaluates it correctly
- Saves the trained model
- Reloads the model for future predictions

---

## 🧠 Problem Type

- **Supervised Learning**
- **Classification**
- Binary outcome:
  - `0` → Benign
  - `1` → Malignant

---

## 📊 Dataset

- Source: `sklearn.datasets.load_breast_cancer`
- Type: Structured medical dataset
- Features: Numeric medical measurements
- Target: Cancer diagnosis (binary)

---

## 🔄 End-to-End Workflow

Load Dataset
↓
Separate Features (X) and Target (y)
↓
Train / Test Split
↓
Pipeline (StandardScaler + Logistic Regression)
↓
Model Training
↓
Predictions on Unseen Data
↓
Model Evaluation
↓
Save Trained Pipeline
↓
Load Pipeline & Predict Again


---

## 🛠 Tools & Technologies Used

- Python
- pandas
- scikit-learn
- matplotlib
- joblib

---

## ⚙️ Model Pipeline

The pipeline combines preprocessing and model training into a single reusable object:

- **StandardScaler** → feature scaling
- **LogisticRegression** → classification model

Using a pipeline ensures:
- No data leakage
- Clean and reusable code
- Production-ready workflow

---

## 📏 Evaluation Metrics

The model is evaluated using:

- Confusion Matrix
- Accuracy
- Precision
- Recall
- ROC AUC

---

## 📈 Results

- Accuracy: ~97%
- ROC AUC: ~0.99
- Very low false negatives (important for medical diagnosis)

These results indicate that the model generalizes well on unseen data.

---

## 💾 Model Persistence

- The trained pipeline is saved using `joblib`
- Saved model file: `cancer_pipeline.joblib`
- The saved model is loaded again to verify it can be reused for predictions

This simulates how models are used in production systems.

---

## 🧠 Key Learnings

- End-to-end ML pipelines are more valuable than standalone models
- Pipelines help prevent data leakage
- Models should be trained once and reused
- Evaluation metrics must be chosen carefully for the problem domain
- ML systems should be reproducible and version-controlled

---

## 🚀 Future Enhancements

- Expose the pipeline using FastAPI
- Add batch prediction support
- Integrate with data pipelines or scheduled jobs
