# Loan Default Prediction — Decision Trees & Random Forest

A machine learning project that predicts whether a borrower will fully repay their loan using **LendingClub** data from 2007–2010. The project compares the performance of a Decision Tree classifier against a Random Forest classifier.

---

## 📁 Project Files

| File | Description |
|------|-------------|
| `loan_data.csv` | Cleaned loan dataset (9,578 records, 14 features) |
| `Saleh-02-Decision_Trees_and_Random_Forest_Project_v2.ipynb` | Main Jupyter Notebook with full analysis |

---

## 📊 Dataset Overview

- **Source:** [LendingClub.com](https://www.lendingclub.com/) (pre-IPO data)
- **Size:** 9,578 rows × 14 columns
- **Target Variable:** `not.fully.paid` (1 = defaulted, 0 = fully repaid)

### Feature Descriptions

| Column | Description |
|--------|-------------|
| `credit.policy` | 1 if the customer meets LendingClub's underwriting criteria, 0 otherwise |
| `purpose` | Purpose of the loan (e.g., credit card, debt consolidation, small business) |
| `int.rate` | Interest rate of the loan as a proportion (e.g., 0.11 = 11%) |
| `installment` | Monthly installment amount owed by the borrower |
| `log.annual.inc` | Natural log of the borrower's self-reported annual income |
| `dti` | Debt-to-income ratio (total debt / annual income) |
| `fico` | FICO credit score of the borrower |
| `days.with.cr.line` | Number of days the borrower has had a credit line |
| `revol.bal` | Revolving balance (unpaid amount at end of billing cycle) |
| `revol.util` | Revolving line utilization rate (credit used / total credit available) |
| `inq.last.6mths` | Number of creditor inquiries in the last 6 months |
| `delinq.2yrs` | Times the borrower was 30+ days past due in the past 2 years |
| `pub.rec` | Number of derogatory public records (bankruptcies, tax liens, judgments) |

---

## 🔧 Requirements

```bash
pip install numpy pandas seaborn matplotlib scikit-learn
```

---

## 🚀 Project Workflow

### 1. Exploratory Data Analysis (EDA)
- FICO score distributions by `credit.policy` outcome
- FICO score distributions by `not.fully.paid` outcome
- Loan count by purpose, colored by repayment status
- Joint plot of FICO score vs. interest rate
- `lmplot` to examine trends across `credit.policy` and `not.fully.paid`

### 2. Data Preprocessing
- One-hot encode the `purpose` categorical column using `pd.get_dummies()` with `drop_first=True`
- Split data into training and testing sets (80/20 split, `random_state=101`)

### 3. Model Training
- **Decision Tree Classifier** — baseline model using default parameters
- **Random Forest Classifier** — ensemble model with `n_estimators=500`

### 4. Evaluation
Both models are evaluated using:
- Classification Report (Precision, Recall, F1-Score)
- Confusion Matrix

---

## 📈 Model Comparison

| Model | Notes |
|-------|-------|
| Decision Tree | Faster to train, simpler, but generally lower accuracy |
| Random Forest | More robust, handles overfitting better with 500 trees |

> The Random Forest model is expected to outperform the single Decision Tree due to ensemble averaging.

---

## 📌 Notes

- The dataset has already been cleaned of NA values.
- The `purpose` column is the only categorical feature and is handled via dummy encoding.
- FICO score is a strong predictor of loan repayment behavior.

---

## 👤 Author

**Saleh** — Machine Learning Course Project
