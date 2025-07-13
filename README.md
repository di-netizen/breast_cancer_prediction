# 🧠 Breast Cancer Prediction using Machine Learning

This project presents a complete machine learning pipeline to predict whether a breast tumor is malignant or benign using diagnostic medical data. It includes data preprocessing, exploratory analysis, model training with evaluation, and a real-time prediction simulation using a trained model.

---

## 📊 Dataset

- **Source:** [UCI Breast Cancer Wisconsin Dataset](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29)
- **Samples:** 569
- **Features:** 30 numerical diagnostic attributes
- **Target Values:**
  - `0` → Malignant (cancerous)
  - `1` → Benign (non-cancerous)

---

## 🧪 Project Workflow

### 1. Data Cleaning (`cancer_step2_clean.py`)
- Loads the raw dataset
- Handles missing values (if any)
- Standardizes features using `StandardScaler`
- Saves cleaned dataset

### 2. Exploratory Data Analysis (`cancer_step3_eda.py`)
- Class distribution plot (0 vs 1)
- Correlation heatmap for top 10 features
- KDE plots for important features

### 3. Model Training and Evaluation (`cancer_step5_evaluate_save.py`)
- Trains a Random Forest Classifier
- Evaluates model performance:
  - Classification report
  - Confusion matrix
  - ROC-AUC curve
- Saves the model to `breast_cancer_rf_model.pkl`

### 4. Prediction on New Data (`cancer_step6_predict.py`)
- Loads the saved model
- Simulates prediction for new patient record
- Displays prediction and confidence level

---

## 📁 Folder Structure


---

## ▶️ How to Run

Run each script in the following order:

```bash
# Step 1: Clean the data
python cancer_step2_clean.py

# Step 2: Perform EDA
python cancer_step3_eda.py

# Step 3: Train and evaluate the model
python cancer_step5_evaluate_save.py

# Step 4: Predict a new case
python cancer_step6_predict.py

## 🔒 License

This project is licensed under the MIT License © 2025 Divya Pawar.

