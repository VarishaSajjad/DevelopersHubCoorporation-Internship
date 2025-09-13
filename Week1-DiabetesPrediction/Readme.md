# 🩺 Diabetes Prediction Using Patient Data

This project demonstrates building a machine learning model to predict diabetes in patients using a structured dataset. It covers data preprocessing, model training, evaluation, and visualization of results.

---

## 📂 Project Structure


---

## 🧪 Objective

- Predict whether a patient has diabetes or not based on health features such as:
  - Glucose level
  - Blood Pressure
  - BMI
  - Age
  - Insulin
  - Skin Thickness
- Learn basic ML workflow: preprocessing → model training → evaluation.  

---

## 🧪 Dataset

- Source: UCI Machine Learning Repository / Kaggle Diabetes Dataset  
- Format: CSV  
- Size: ~768 rows, 8 features + target column (`Outcome`)  
- Preprocessing Steps:
  - Fill missing values (if any)  
  - Normalize numeric features  
  - Split into training and test sets  

---

## 🧪 Model

- Algorithm: **Logistic Regression / Random Forest / Decision Tree** (example in notebook)  
- Features used: All relevant patient health measurements  
- Target: Binary classification (Diabetic / Non-Diabetic)  

---

## 📊 Evaluation

- Metrics: **Accuracy, Precision, Recall, F1 Score**  
- Visualizations:  
  - Confusion Matrix  
  - ROC Curve (if implemented)  
  - Feature Importance (if using tree-based models)  

---

## 🚀 How to Run

1. Clone the repository or download the folder.
2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn

## 🛠️ Tech Stack

Python 3.x

Pandas, NumPy

Scikit-learn

Matplotlib, Seaborn

#Author: Varisha Sajjad