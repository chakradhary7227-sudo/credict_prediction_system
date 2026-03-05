# Credit Default Prediction System

## 📌 Project Overview

The **Credit Default Prediction System** is a Machine Learning project designed to predict whether a credit card customer is likely to default on their payment in the next month. Predicting credit default risk helps financial institutions make better lending decisions, reduce financial losses, and manage risk effectively.

This project demonstrates an **end-to-end machine learning pipeline**, including data preprocessing, feature engineering, model training, hyperparameter tuning, and model evaluation.

---

## 🎯 Objectives

* Apply **data preprocessing and feature engineering** techniques on real-world financial data
* Train and compare multiple **classification models**
* Perform **hyperparameter tuning using cross-validation**
* Evaluate model performance using appropriate **classification metrics**
* Build a **reproducible machine learning pipeline**
* Prepare the trained model for **future deployment**

---

## 📂 Dataset

The project uses the **UCI Credit Card Default Dataset**, which contains financial and demographic information about credit card clients.

### Key Features in the Dataset

* **LIMIT_BAL** – Credit limit of the customer
* **SEX** – Gender of the customer
* **EDUCATION** – Education level
* **MARRIAGE** – Marital status
* **AGE** – Age of the customer

### Financial Behavior Features

* **PAY_0 – PAY_6** – Repayment status over the last 6 months
* **BILL_AMT1 – BILL_AMT6** – Bill amounts for the last 6 months
* **PAY_AMT1 – PAY_AMT6** – Payment amounts for the last 6 months

### Target Variable

* **default.payment.next.month**

  * `0` → No default
  * `1` → Default

---

## ⚙️ Technologies Used

* **Python**
* **Google Colab**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **XGBoost**
* **Joblib**

---

## 📊 Project Workflow

### 1. Exploratory Data Analysis (EDA)

* Analyzed dataset structure and statistical summary
* Visualized feature distributions
* Studied correlation between features and target variable
* Identified potential patterns in customer payment behavior

### 2. Data Preprocessing

* Checked for missing values
* Feature scaling using **StandardScaler**
* Train-test dataset splitting
* Prepared clean data for model training

### 3. Feature Engineering

Additional features were created to improve model performance:

* **Total Bill Amount**
* **Total Payment Amount**
* **Credit Utilization Ratio**

These features help capture a customer's financial behavior more effectively.

### 4. Model Development

Multiple machine learning models were trained and compared:

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost

### 5. Hyperparameter Tuning

Used **GridSearchCV with cross-validation** to find the best parameters for the model and improve prediction accuracy.

### 6. Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC Score
* Confusion Matrix

These metrics help assess both **statistical performance** and **business relevance** of the model.

### 7. Model Saving

The best-performing model was saved using **Joblib** for future deployment or integration into applications.

---

## 📁 Project Structure

```
Credit-Default-Prediction/
│
├── Notebook1_EDA_Preprocessing.ipynb
├── Notebook2_Model_Development.ipynb
├── Notebook3_Model_Evaluation.ipynb
│
├── dataset/
│   └── credit_card_default.csv
│
├── models/
│   └── best_model.pkl
│
└── README.md
```

---

## 🚀 Results

After comparing multiple machine learning models, the best-performing model was selected based on **ROC-AUC score and classification metrics**. The model can effectively predict whether a customer is likely to default based on their past financial behavior.

---

## 📈 Future Improvements

* Deploy the model using **Streamlit or Flask**
* Add **real-time prediction interface**
* Apply **advanced feature selection techniques**
* Integrate **MLOps tools for experiment tracking**

---

## 👨‍💻 Author

**Chakradhar Y**

B.Tech – Computer Science Engineering (AI Specialization)

Interested in **Machine Learning, Artificial Intelligence, and Data Science**, and building practical solutions using data-driven approaches.
