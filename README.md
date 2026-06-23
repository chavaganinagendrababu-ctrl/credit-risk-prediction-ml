# Credit Risk Prediction Using Machine Learning

## Overview

This project develops a Machine Learning solution to predict loan approval decisions based on applicant financial and demographic information. The objective is to assist financial institutions in reducing lending risk and improving decision-making through data-driven insights.

---

## Business Problem

Banks receive numerous loan applications daily. Approving loans for high-risk applicants can lead to financial losses, while rejecting eligible applicants can result in missed business opportunities.

The goal of this project is to build a predictive model that can determine whether a loan application should be approved or rejected.

---

## Dataset Information

* Total Records: 614
* Target Variable: Loan_Status

  * Y = Approved
  * N = Rejected

### Features

* Gender
* Married
* Dependents
* Education
* Self_Employed
* ApplicantIncome
* CoapplicantIncome
* LoanAmount
* Loan_Amount_Term
* Credit_History
* Property_Area

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost
* Google Colab

---

## Project Workflow

### Data Preprocessing

* Handled missing values
* Performed data cleaning
* Removed unnecessary columns
* Encoded categorical variables

### Exploratory Data Analysis (EDA)

* Loan approval distribution
* Credit history analysis
* Income analysis
* Property area analysis
* Education analysis

### Feature Engineering

Created a new feature:

```python
Total_Income = ApplicantIncome + CoapplicantIncome
```

### Model Development

Implemented and evaluated:

* Logistic Regression
* Random Forest
* XGBoost
* Gaussian Naive Bayes
* Tuned Random Forest (GridSearchCV)

---

## Model Performance

| Model                | Accuracy |
| -------------------- | -------- |
| Logistic Regression  | 78.86%   |
| Random Forest        | 77.24%   |
| XGBoost              | 77.24%   |
| Gaussian Naive Bayes | 78.86%   |
| Tuned Random Forest  | 78.86%   |

### Final Selected Model

**Logistic Regression**

Training Accuracy: **81.67%**

Testing Accuracy: **78.86%**

Model Status: **Good Fit**

---

## Feature Importance Analysis

### Top Factors Influencing Loan Approval

| Feature           | Importance |
| ----------------- | ---------- |
| Credit_History    | 25.8%      |
| Total_Income      | 15.9%      |
| LoanAmount        | 14.7%      |
| ApplicantIncome   | 14.5%      |
| CoapplicantIncome | 8.7%       |

---

## Key Business Insights

* Credit History is the strongest predictor of loan approval.
* Applicants with higher income have a greater probability of approval.
* Total household income significantly influences lending decisions.
* Loan amount impacts approval likelihood.
* Financial factors contribute more than demographic factors.

---

## Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

### Logistic Regression Results

Training Accuracy: 81.67%

Testing Accuracy: 78.86%

Difference: 2.81%

The small difference between training and testing accuracy indicates that the model generalizes well and does not suffer from significant overfitting.

---

## Project Structure

```text
Credit-Risk-Prediction-ML/
│
├── data/
│   ├── train.csv
│   └── test.csv
│
├── notebooks/
│   └── Credit_Risk_Prediction.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/chavaganinagendrababu-ctrl/credit-risk-prediction-ml.git
```

Navigate to the project directory:

```bash
cd credit-risk-prediction-ml
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the notebook and execute all cells.

---

## Future Enhancements

* Power BI Dashboard Development
* Streamlit Web Application
* SHAP Explainability
* ROC-AUC Analysis
* Cloud Deployment
* Real-Time Loan Prediction API

---
