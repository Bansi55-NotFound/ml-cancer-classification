# Machine Learning Classification Projects

This repository contains end-to-end machine learning classification projects built using Python and scikit-learn.

## Projects

### 1. Cancer Classification
- Logistic Regression model
- Evaluation using confusion matrix, precision, recall, accuracy, ROC–AUC
- Focus on medical error analysis

### 2. Heart Disease Prediction
- Logistic Regression model
- Feature scaling and proper tra# 🔬 ML Classification Projects

> End-to-end machine learning classification projects built with Python and scikit-learn — with a focus on proper model evaluation and medical error analysis.

---

## 📂 Projects

### 1. 🎗️ Breast Cancer Classification

Predicts whether a breast tumor is malignant or benign using the Breast Cancer Wisconsin dataset.

| Property | Detail |
|----------|--------|
| Algorithm | Logistic Regression |
| Dataset | Breast Cancer Wisconsin (sklearn) |
| Features | 30 numerical features |
| Target | Binary: malignant (0) / benign (1) |

**Evaluation focus:** Medical classification demands low false negatives (missing a cancer is worse than a false alarm). This project analyzes the confusion matrix with that lens — prioritizing recall for the malignant class.

**Metrics used:**
- Confusion Matrix
- Precision & Recall
- Accuracy
- ROC-AUC

---

### 2. ❤️ Heart Disease Prediction

Predicts the likelihood of heart disease based on clinical features.

| Property | Detail |
|----------|--------|
| Algorithm | Logistic Regression |
| Features | Clinical indicators (age, cholesterol, etc.) |
| Target | Binary: disease present / absent |

**Includes:** Feature scaling, proper train/test split, and evaluation using accuracy, precision, recall, and ROC-AUC.

---

## ⚙️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/Bansi55-NotFound/ml-cancer-classification.git
cd ml-cancer-classification

# 2. Create and activate virtual environment
python -m venv venv
source venv/bin/activate       # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Open the notebooks
jupyter notebook
```

---

## 🛠️ Tech Stack

- **Python** — Core language
- **scikit-learn** — Model training and evaluation
- **Pandas & NumPy** — Data manipulation
- **Matplotlib / Seaborn** — Visualization
- **Jupyter Notebook** — Exploratory analysis

---

## 💡 Key Learnings

- Why accuracy alone is misleading for imbalanced medical datasets
- How to interpret confusion matrices in a clinical context
- The importance of recall vs precision depending on the cost of false negatives
- Proper train/test splitting to avoid data leakage
in/test split
- Evaluation using accuracy, precision, recall, ROC–AUC

## Tools & Skills
- Python
- Pandas, NumPy
- scikit-learn
- Model evaluation and error analysis
- Git & GitHub
