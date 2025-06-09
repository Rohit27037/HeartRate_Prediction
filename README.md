# HeartRate_Prediction
Project for EDGENIUS SKILLFIED MENTOR PRIVATE LIMITED

# ❤️ Heart Rate Prediction using Framingham Dataset

This project uses machine learning to predict whether an individual's heart rate is elevated based on features from the **Framingham Heart Study** dataset.

## 📌 Objective

To build a classification model that predicts **elevated vs. normal heart rate** using simple medical and lifestyle data.

## 📁 Dataset: framingham.csv

The Framingham Heart Study dataset includes data on cardiovascular health, such as:

- Age  
- Blood Pressure  
- BMI  
- Glucose  
- Smoking habits  
- Heart Rate (our target)

We classify heart rate into two categories:
- **Elevated** (e.g., ≥ 90 bpm)
- **Normal** (e.g., < 90 bpm)

> ⚠️ Note: You can adjust this threshold based on clinical definitions or project needs.

## 🧪 Model Used

- **Logistic Regression**
  - Used for binary classification of heart rate status.

## 🛠️ Workflow

1. **Data Loading & Cleaning**
   - Read `framingham.csv`
   - Drop missing or null values

2. **Feature Selection**
   - Key predictors: `age`, `BMI`, `glucose`, `sysBP`, `diaBP`, `cigsPerDay`

3. **Label Engineering**
   - Created a binary `heart_rate_status` column:
     - 1: Elevated
     - 0: Normal

4. **Preprocessing**
   - Feature scaling (StandardScaler)
   - Train-test split

5. **Model Training**
   - Trained Logistic Regression classifier on selected features

6. **Model Evaluation**
   - Accuracy score
   - Confusion matrix
   - Precision, Recall, F1-score

7. **Visualization**
   - Correlation heatmap
   - Distribution plots

## 📊 Results

- The model predicts heart rate status with reasonable accuracy.
- Balanced performance on sensitivity and specificity.

## 📎 Requirements

Install these Python packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
