# Demo Project: Bank Marketing Campaign Prediction

**Type:** Classification  
**Weeks Covered:** 6-7  
**Dataset:** [Bank Marketing (UCI ML Repository)](https://archive.ics.uci.edu/ml/datasets/bank+marketing)

---

## 🎯 Project Overview

This demonstration project walks through a complete classification pipeline to predict whether a client will subscribe to a term deposit. We'll follow the same 7-stage CRISP-DM methodology you'll use for your capstone project.

### Business Problem

> **Goal:** Predict whether a client will subscribe to a term deposit (yes/no) based on client demographics, campaign information, and economic indicators.

This is a binary classification problem that demonstrates key concepts including handling class imbalance, categorical encoding, and evaluating classification models beyond accuracy.

---

## 📊 Dataset Description

The Bank Marketing dataset contains data from direct marketing campaigns (phone calls) of a Portuguese banking institution.

### Client Features

| Feature | Description | Type |
|---------|-------------|------|
| `age` | Client age | Numeric |
| `job` | Type of job | Categorical |
| `marital` | Marital status | Categorical |
| `education` | Education level | Categorical |
| `default` | Has credit in default? | Binary |
| `housing` | Has housing loan? | Binary |
| `loan` | Has personal loan? | Binary |

### Campaign Features

| Feature | Description | Type |
|---------|-------------|------|
| `contact` | Contact communication type | Categorical |
| `month` | Last contact month | Categorical |
| `day_of_week` | Last contact day | Categorical |
| `duration` | Last contact duration (seconds) | Numeric |
| `campaign` | Contacts during this campaign | Numeric |
| `pdays` | Days since last contact | Numeric |
| `previous` | Contacts before this campaign | Numeric |
| `poutcome` | Outcome of previous campaign | Categorical |

### Economic Indicators

| Feature | Description | Type |
|---------|-------------|------|
| `emp.var.rate` | Employment variation rate | Numeric |
| `cons.price.idx` | Consumer price index | Numeric |
| `cons.conf.idx` | Consumer confidence index | Numeric |
| `euribor3m` | Euribor 3-month rate | Numeric |
| `nr.employed` | Number of employees | Numeric |

**Target Variable:** `y` — Has the client subscribed to a term deposit? (yes/no)

---

## ⚠️ Key Challenge: Class Imbalance

The dataset is **imbalanced**: approximately 88% "no" vs 12% "yes". This is realistic for marketing campaigns but requires special handling:

- Stratified sampling
- Class weights
- SMOTE (Synthetic Minority Over-sampling)
- Appropriate metrics (not just accuracy!)

---

## 📁 Notebooks

| Notebook | Description | Week |
|----------|-------------|------|
| [01_eda.ipynb](01_eda.ipynb) | Exploratory Data Analysis | 6 |
| [02_feature_engineering.ipynb](02_feature_engineering.ipynb) | Feature Engineering & Data Prep | 6-7 |
| [03_modeling.ipynb](03_modeling.ipynb) | Model Building & Evaluation | 7 |

---

## 🔧 Key Techniques Demonstrated

### EDA (Week 6)
- Class distribution analysis
- Feature distributions by target class
- Correlation analysis with categorical variables
- Identifying data quality issues

### Feature Engineering (Week 6-7)
- One-hot encoding for categorical variables
- Ordinal encoding for ordered categories
- Handling "unknown" values
- Feature scaling
- Stratified train/test split

### Modeling (Week 7)
- Logistic Regression (baseline)
- Decision Tree Classifier
- Random Forest Classifier
- Handling class imbalance (class_weight, SMOTE)
- Cross-validation with stratification
- Hyperparameter tuning

### Evaluation Metrics

For imbalanced classification, we focus on:

| Metric | Why It Matters |
|--------|----------------|
| **Precision** | Of predicted "yes", how many were correct? |
| **Recall** | Of actual "yes", how many did we catch? |
| **F1-Score** | Harmonic mean of precision and recall |
| **ROC-AUC** | Overall discriminative ability |
| **Confusion Matrix** | Visual breakdown of predictions |

> ⚠️ **Accuracy alone is misleading!** A model predicting all "no" would be 88% accurate but useless.

---

## 🚀 Running the Notebooks

```bash
# Clone the course materials repo
git clone https://github.com/MTSU-DATA4950-Capstone-Spring2026/course-materials.git
cd course-materials/demos/bank-marketing-classification

# Install dependencies
pip install -r requirements.txt

# Download the dataset (if not included)
# Visit: https://archive.ics.uci.edu/ml/datasets/bank+marketing

# Launch Jupyter
jupyter notebook
```

---

## 📦 Requirements

```
pandas>=2.0.0
numpy>=1.24.0
scikit-learn>=1.3.0
imbalanced-learn>=0.11.0
matplotlib>=3.7.0
seaborn>=0.12.0
jupyter>=1.0.0
```

---

## 📚 References

- [UCI ML Repository - Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing)
- [Moro et al., 2014 - Original Research Paper](https://repositorio.iscte-iul.pt/bitstream/10071/9499/5/dss_v3.pdf)

---

*This demo is part of DATA 4950: Data Science Capstone — Spring 2026*
