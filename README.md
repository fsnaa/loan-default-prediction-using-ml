
# Loan Default Prediction using Machine Learning

A machine learning project to predict whether a borrower is likely to default on a loan, using financial and demographic data. Built to help financial institutions minimize lending risk and make smarter credit decisions.

---

## Problem Statement

Loan default is a critical challenge in the financial industry. The goal of this project is to build a classification model that identifies high-risk borrowers before a loan is issued — reducing financial loss and improving decision-making.

---

## Project Workflow

1. **Data Overview & Understanding** — explored the dataset structure, data types, and distributions
2. **Data Cleaning & Preprocessing** — handled missing values, removed inconsistencies, and prepared the data for modeling
3. **Feature Engineering** — created meaningful financial indicators:
   - Income-to-Loan Ratio
   - EMI (Equated Monthly Installment)
   - Credit-to-Loan Ratio
4. **Modeling** — built a Logistic Regression classification model
5. **Class Imbalance Handling** — addressed imbalance to improve detection of actual defaulters
6. **Evaluation** — assessed model using Accuracy, Precision, and Recall

---

## Model Performance

| Metric | Score |
|--------|-------|
| Accuracy | 68.05% |
| Precision | 22.05% |
| Recall | **69.64%** |

### Why Recall matters here

In financial risk applications, **missing a defaulter (false negative) is far more costly** than flagging a non-defaulter (false positive). By prioritizing Recall, the model correctly identifies ~70% of actual defaulters — making it more useful in real-world lending scenarios, even at the cost of lower precision.

---

## Tools & Technologies

| Category | Tools |
|----------|-------|
| Language | Python |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Modeling | Scikit-learn (Logistic Regression) |
| Environment | Jupyter Notebook |

---

## Key Insights

- Feature engineering significantly improved model interpretability and performance
- Class imbalance handling reduced false negatives and increased true positive detection
- The trade-off between Precision and Recall is acceptable — in finance, catching risky borrowers matters more than avoiding false alarms

---

## Project Structure

```
loan-default-prediction/
│
├── data/                  # Dataset files
├── notebooks/             # Jupyter Notebooks
│   └── loan_default.ipynb
├── README.md
└── requirements.txt
```

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/fsnaa/loan-default-prediction.git

# Navigate to the project
cd loan-default-prediction

# Install dependencies
pip install -r requirements.txt

# Open the notebook
jupyter notebook notebooks/loan_default.ipynb
```

---

## Author

**Fasna**
[LinkedIn](https://www.linkedin.com/in/fasna-s/) | [GitHub](https://github.com/fsnaa)
