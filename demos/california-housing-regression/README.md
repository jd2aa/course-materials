# Demo Project: California Housing Price Prediction

**Type:** Regression  
**Weeks Covered:** 4-5  
**Dataset:** [California Housing (sklearn)](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html)

---

## 🎯 Project Overview

This demonstration project walks through a complete regression pipeline to predict median house values in California districts. We'll follow the same 7-stage CRISP-DM methodology you'll use for your capstone project.

### Business Problem

> **Goal:** Predict the median house value for California districts based on demographic and geographic features.

This is a classic regression problem that demonstrates key concepts including feature engineering, handling skewed distributions, and evaluating regression models.

---

## 📊 Dataset Description

The California Housing dataset contains 20,640 observations with 8 features:

| Feature | Description |
|---------|-------------|
| `MedInc` | Median income in block group |
| `HouseAge` | Median house age in block group |
| `AveRooms` | Average number of rooms per household |
| `AveBedrms` | Average number of bedrooms per household |
| `Population` | Block group population |
| `AveOccup` | Average number of household members |
| `Latitude` | Block group latitude |
| `Longitude` | Block group longitude |

**Target Variable:** `MedHouseVal` — Median house value (in $100,000s)

---

## 📁 Notebooks

| Notebook | Description | Week |
|----------|-------------|------|
| [01_eda.ipynb](01_eda.ipynb) | Exploratory Data Analysis | 4 |
| [02_feature_engineering.ipynb](02_feature_engineering.ipynb) | Feature Engineering & Data Prep | 4-5 |
| [03_modeling.ipynb](03_modeling.ipynb) | Model Building & Evaluation | 5 |

---

## 🔧 Key Techniques Demonstrated

### EDA (Week 4)
- Distribution analysis of target variable
- Correlation heatmaps
- Geographic visualization (lat/long)
- Identifying outliers

### Feature Engineering (Week 4-5)
- Creating new features (rooms per person, bedroom ratio)
- Handling skewed distributions
- Feature scaling
- Train/test split strategies

### Modeling (Week 5)
- Linear Regression (baseline)
- Ridge & Lasso Regression
- Random Forest Regressor
- Cross-validation
- Hyperparameter tuning with GridSearchCV

### Evaluation Metrics
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score
- Residual analysis

---

## 🚀 Running the Notebooks

```bash
# Clone the course materials repo
git clone https://github.com/MTSU-DATA4950-Capstone-Spring2026/course-materials.git
cd course-materials/demos/california-housing-regression

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

---

## 📦 Requirements

```
pandas>=2.0.0
numpy>=1.24.0
scikit-learn>=1.3.0
matplotlib>=3.7.0
seaborn>=0.12.0
jupyter>=1.0.0
```

---

## 📚 References

- [Scikit-learn California Housing Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html)
- [Original Dataset Paper (Pace & Barry, 1997)](https://www.sciencedirect.com/science/article/abs/pii/S016771529600140X)

---

*This demo is part of DATA 4950: Data Science Capstone — Spring 2026*
