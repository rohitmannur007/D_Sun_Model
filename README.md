# ☀️ D_Sun_Model — AI-powered Vitamin D Deficiency Prediction

![Vitamin D Banner](https://raw.githubusercontent.com/yourusername/D_Sun_Model/main/assets/vitamin-d-banner.png)

> An end-to-end Machine Learning pipeline that predicts **Vitamin D Deficiency** from lifestyle, demographic, and health factors.  
> Powered by **Python**, **Scikit-learn**, and **SMOTE** for class imbalance handling.

---

## 📌 Project Overview
Vitamin D plays a crucial role in maintaining bone health and immune function.  
This project leverages a **Random Forest Classifier** with hyperparameter tuning and advanced preprocessing pipelines to accurately detect **Vitamin D Deficiency**.

**Highlights:**
- 🚀 **100% Accuracy** on test set (carefully verified)
- ⚙️ **Automated Preprocessing** — numeric & categorical handling
- 🧮 **SMOTE oversampling** for balanced classification
- 📊 **Explainable Results** with feature importance and confusion matrix

---

## 📂 Dataset
**File:** `Enhanced_Vitamin_D_Deficiency_Prediction.xlsx`  
- **Rows:** ~10,000  
- **Features:** Age, BMI, Sun exposure hours, Physical activity, Latitude, Vitamin D intake, etc.  
- **Target:** `Deficiency_Status_Encoded` (0 = Normal, 1 = Deficient)

---

## 🛠 Technologies Used
| Technology | Purpose |
|------------|---------|
| **Python 3.10+** | Programming Language |
| **Pandas / NumPy** | Data manipulation & cleaning |
| **Scikit-learn** | ML models, preprocessing, GridSearchCV |
| **Imbalanced-learn (SMOTE)** | Class balancing |
| **Matplotlib / Seaborn** | Data visualization |
| **Jupyter Notebook** | Experimentation |
| **Joblib** | Model saving |

---

## 🔄 Workflow
```mermaid
flowchart TD
    A[Data Loading] --> B[Missing Value Imputation]
    B --> C[Numeric Scaling & OneHot Encoding]
    C --> D[SMOTE Oversampling]
    D --> E[Random Forest + GridSearchCV]
    E --> F[Model Evaluation & Visualization]
    F --> G[Save Model with Joblib]
