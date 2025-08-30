# 🩺 Diabetes Prediction with Feature Engineering

This project aims to predict the likelihood of diabetes in individuals based on various health indicators using machine learning. Before modeling, extensive exploratory data analysis and feature engineering steps were applied to improve model performance and interpretability.

---

## Objective

- Predict whether a person has diabetes (`Outcome`) using numerical health features.
- Apply systematic feature engineering and preprocessing steps.
- Build a machine learning model using a clean and enriched dataset.

---

## 📁 Dataset

The dataset comes from the **US National Institute of Diabetes and Digestive and Kidney Diseases**, and includes:

- `Pregnancies`: Number of times pregnant  
- `Glucose`: Plasma glucose concentration  
- `BloodPressure`: Diastolic blood pressure (mm Hg)  
- `SkinThickness`: Triceps skin fold thickness (mm)  
- `Insulin`: 2-Hour serum insulin (mu U/ml)  
- `BMI`: Body mass index  
- `DiabetesPedigreeFunction`: Diabetes pedigree function  
- `Age`: Age in years  
- `Outcome`: Class variable (0 or 1), indicates diabetes

---

## ⚙️ Technologies Used

- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn

---

## Main Steps

### 1. Exploratory Data Analysis
- Checked data structure, types, and value ranges
- Visualized distributions and correlations
- Identified categorical vs. numerical variables

### 2. Data Preprocessing
- Replaced impossible values (e.g., 0 for glucose or insulin) with `NaN`
- Filled missing values with median imputation
- Detected and capped outliers

### 3. Feature Engineering
- Created new features based on age, BMI, glucose, and their combinations
- Designed categorical bins to capture hidden patterns
- Generated interaction features (e.g., `Glucose * Pregnancies`)

### 4. Encoding & Scaling
- Applied Label Encoding and One-Hot Encoding
- Standardized numerical features with `StandardScaler`

### 5. Modeling
- Used **Random Forest Classifier**
- Evaluated using Accuracy, Recall, Precision, F1 Score, and AUC
- Plotted feature importances

---

## ✅ Sample Output

```text
Accuracy: 0.79  
Recall: 0.711  
Precision: 0.67  
F1 Score: 0.69  
AUC Score: 0.77
```

---

## 🚀 How to Run

Make sure you have Python and the required libraries installed.

Then, run the main script:

```bash
python diabetes_prediction.py
```
