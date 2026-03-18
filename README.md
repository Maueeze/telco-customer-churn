# Telco Customer Churn Prediction

## 📁 Project Structure

```
telco-customer-churn/
├── data/                  # raw dataset
│   └── Telco_Customer_Churn.csv
├── notebook/              # main analysis and modelling
│   └── telco_customer_churn.ipynb
├── README.md              # project description
├── requirements.txt       # dependencies
└── .gitignore
```


## 📌 Project Overview

This project focuses on analysing and predicting customer churn in a telecommunications company.

The goal is to:

* understand key drivers of churn,
* build machine learning models to predict customer behaviour,
* compare model performance and interpret results.

---

## 📊 Dataset

The dataset contains information about ~7000 customers, including:

* demographic data,
* services used,
* billing information,
* churn status.

Target variable:

* `Churn` (Yes / No)

---

## 🔍 Key Insights from EDA

The exploratory analysis revealed that churn is strongly associated with:

* **contract type** (month-to-month customers churn the most),
* **customer tenure** (shorter tenure → higher churn),
* **monthly charges** (higher charges → higher churn),
* **lack of support services** (no TechSupport / OnlineSecurity),
* **payment method** (electronic check users churn more).

---

## ⚙️ Modeling Approach

The following models were trained and compared:

* Logistic Regression
* Decision Tree
* Random Forest

All models used a shared preprocessing pipeline:

* missing value imputation,
* scaling for numerical features,
* one-hot encoding for categorical variables.

Evaluation metrics:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC

---

## 📈 Results

* Logistic Regression achieved the highest **ROC-AUC** and **recall**.
* Decision Tree achieved the highest **accuracy**.
* Random Forest performed well but did not outperform Logistic Regression.

---

## ✅ Final Model Choice

Logistic Regression was selected as the final model because:

* it provides the best balance between performance and interpretability,
* it detects more churned customers (high recall),
* it allows a clear explanation of churn drivers.

---

## 🧠 Key Takeaways

* Customer churn is strongly influenced by contract type and tenure.
* Service-related features (TechSupport, OnlineSecurity) are important predictors.
* Interpretable models can be very effective in business use cases.

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Matplotlib
* scikit-learn

---

## 🚀 Future Improvements

* hyperparameter tuning,
* threshold optimization,
* cross-validation,
* adding more advanced models (e.g. Gradient Boosting),
* business cost-based evaluation.

---
