# California Housing Dataset - README

## What is This Data?

Raw housing dataset with 20,640 houses from California (1990 Census).

**File:** `california_housing.csv`

---

## Quick Facts

| Item | Details |
|------|---------|
| Records | 20,640 houses |
| Variables | 9 (8 features + 1 target) |
| File Size | ~2 MB |
| Missing Values | 0 (none!) |
| Source | 1990 U.S. Census |

---

## The Variables (What Each Column Means)

### Features (What we use to predict)

| Name | What It Means | Example |
|------|--------------|---------|
| **MedInc** | Median household income (×$10k) | 3.5 = $35,000 |
| **HouseAge** | Median house age (years) | 25 = 25 years old |
| **AveRooms** | Average rooms per house | 6 = 6 rooms |
| **AveBedrms** | Average bedrooms per house | 1.5 = 1.5 bedrooms |
| **Population** | Total people in area | 1000 = 1,000 people |
| **AveOccup** | Average people per house | 3 = 3 people/house |
| **Latitude** | North-South position | 37.8 = Northern CA |
| **Longitude** | East-West position | -122.2 = Western CA |

### Target (What we're predicting)

| Name | What It Means | Example |
|------|--------------|---------|
| **MedHouseVal** | Median house value (×$100k) | 3.5 = $350,000 |

---

## How to Load This Data

### Method 1: Using Pandas (Recommended)

```python
import pandas as pd

# Load the data
df = pd.read_csv('data/raw/california_housing.csv')

# Check shape
print(df.shape)  # Should be (20640, 9)

# View first few rows
print(df.head())

# Basic statistics
print(df.describe())
```

### Method 2: Using scikit-learn (Original Source)

```python
from sklearn.datasets import fetch_california_housing

# Download from original source
housing = fetch_california_housing(as_frame=True)
df = housing.frame

# View the data
print(df.head())
```

---

## Important Rules

✅ **DO:**
- Read this README first
- Explore data in notebooks
- Clean data before modeling
- Create processed copies

❌ **DON'T:**
- Modify housing.csv directly
- Skip data cleaning
- Use raw data in models
- Delete data without investigating

---

## Next Steps

1. **Explore:** See `notebooks/01_EDA.ipynb`