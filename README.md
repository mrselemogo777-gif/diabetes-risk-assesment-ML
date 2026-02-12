#  Diabetes Risk Assessment – End-to-End Machine Learning Pipeline

An end-to-end machine learning pipeline for diabetes risk assessment and patient stratification using the BRFSS 2015 public health dataset.  

This project integrates data preprocessing, exploratory data analysis, feature engineering, clustering, and predictive modeling to demonstrate how machine learning can support early disease detection and healthcare analytics.

---

##  Project Objective

The objective of this project is to design and implement a structured machine learning workflow capable of:

- Predicting diabetes risk from demographic and clinical indicators  
- Stratifying patients into Low, Medium, and High-risk groups  
- Evaluating model performance under class imbalance  
- Demonstrating practical ML applications in public health analytics  

The system illustrates how predictive modeling can support early intervention strategies and data-driven healthcare decision-making.

---

##  Demo Video

[![Watch the Demo](https://img.youtube.com/vi/hsJrlKPwQ28/0.jpg)](https://www.youtube.com/watch?v=hsJrlKPwQ28)

---

##  Key Features

- Data cleaning and duplicate removal  
- Exploratory Data Analysis (EDA) with statistical and visual insights  
- Feature Engineering:
  - Health Risk Score (HighBP + HighChol)
  - BMI Category Classification  
- Patient Risk Clustering (Low / Moderate / High Risk)
- Supervised Machine Learning Models:
  - Logistic Regression
  - Random Forest
  - Linear Support Vector Machine (SVM)
  - Artificial Neural Network (ANN)
- ROC Curve analysis and classification metrics
- 3D visualization of risk stratification patterns

---

##  Machine Learning Workflow

Raw Data  
→ Data Cleaning  
→ Feature Engineering  
→ Risk Clustering  
→ Model Training  
→ Model Evaluation  
→ Risk Prediction & Interpretation  

---

## Model Performance

The dataset exhibits class imbalance, with diabetes prevalence of approximately **15.3%**, making evaluation metrics beyond accuracy essential.

### Logistic Regression (Test Set)

- Accuracy: **84.8%**
- Precision: **51.5%**
- Recall (Sensitivity): **5.3%**
- F1 Score: **9.6%**
- ROC-AUC Score: **0.772**

### Model Comparison (Cross-Validation Accuracy)

- Logistic Regression: **~84.7%**
- Random Forest: **~84.7%**
- Linear SVM: **~84.6%**
- ANN: **~84.1%**

### Interpretation

- High overall accuracy reflects strong identification of non-diabetic cases.
- ROC-AUC of 0.772 indicates solid discriminatory performance.
- Low recall highlights the impact of class imbalance and the need for techniques such as threshold tuning or class weighting in medical screening systems.
- Accuracy alone is not sufficient due to imbalance; AUC and sensitivity provide more meaningful evaluation in healthcare contexts.

---

##  Dataset

**BRFSS 2015 – Behavioral Risk Factor Surveillance System**  
Source: https://www.cdc.gov/brfss/

The dataset contains demographic, behavioral, and clinical health indicators collected across the United States and is widely used for public health research.

---

## Technology Stack

- Python 3.x  
- Pandas & NumPy  
- Scikit-learn  
- Matplotlib & Seaborn  
- TensorFlow / Keras (Neural Networks)  
- Jupyter Notebook  

---

##  Installation & Setup

```bash
# Clone the repository
git clone https://github.com/mrselemogo777-gif/diabetes-risk-assesment-ML.git

# Navigate into the project directory
cd diabetes-risk-assesment-ML

# Install dependencies
pip install -r requirements.txt
