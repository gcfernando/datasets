# 🌟 Dataset Playground — Machine Learning Datasets for Practice (CSV)

Explore nine **CSV datasets for machine learning practice**, data cleaning, feature engineering, and exploratory data analysis (EDA). The collection includes classification, regression, text sentiment and time-series exercises — from **Iris** and **Titanic** to messy customer, sales, review and sensor tables. Choose a file in the catalog below, then use the pandas quick start to load it locally or from GitHub. Dataset provenance and license information is incomplete; see the [source and reuse notes](#source-and-reuse-notes).

## ✨ What’s inside?

This repo contains 9 structured datasets across common ML scenarios:

- Customer behavior and spend prediction
- Fraud detection
- Sentiment analysis
- Time-series forecasting
- Classic ML benchmark datasets
- Business-themed practice tables and established teaching datasets

---

## 📏 Size at a Glance

| File | Rows | Columns |
|---|---:|---:|
| `customer_data.csv` | 1,000 | 9 |
| `sales_data.csv` | 1,000 | 8 |
| `reviews_data.csv` | 1,000 | 6 |
| `sensor_data.csv` | 1,000 | 5 |
| `College.csv` | 777 | 19 (the first, unnamed column holds the college name) |
| `Iris.csv` | 150 | 5 |
| `Purchase.csv` | 10 | 4 |
| `Salary.csv` | 205 | 2 |
| `Titanic.csv` | 891 | 12 |

Row counts exclude the header row.

---

## 📊 Dataset Catalog

| File | Theme | Problem Type | Target/Goal | Best For |
|---|---|---:|---|---|
| [customer_data.csv](customer_data.csv) | Customer analytics | Regression | Predict `Purchase_Amount` | EDA, data cleaning, feature engineering |
| [sales_data.csv](sales_data.csv) | Transactions | Classification | Detect `Is_Fraudulent` | Fraud detection, anomaly handling |
| [reviews_data.csv](reviews_data.csv) | Product feedback | Multiclass classification | Predict review sentiment | NLP, text preprocessing |
| [sensor_data.csv](sensor_data.csv) | IoT sensor readings | Regression | Predict `Temperature` / `Humidity` | Time-series modeling, missing data handling |
| [College.csv](College.csv) | Higher education | Classification | Predict college outcomes / categories (for example `Private`) | Feature selection, logistic regression |
| [Iris.csv](Iris.csv) | Botanical dataset | Classification | Identify flower species | Beginner ML, clustering, classification |
| [Purchase.csv](Purchase.csv) | Customer purchase behavior | Classification | Predict purchase decision | Marketing analytics |
| [Salary.csv](Salary.csv) | Employment dataset | Regression | Predict salary from experience | Linear regression, simple modeling |
| [Titanic.csv](Titanic.csv) | Passenger data | Classification | Predict survival | Data wrangling, binary classification |

---

## 🧩 Detailed Dataset Overview

### 1) `customer_data.csv` — Customer Spending Data
**Focus:** Missing values, duplicates, inconsistent data, categorical encoding, text cleaning  
**Target:** `Purchase_Amount`  
**Problem type:** Regression  
**Goal:** Predict how much a customer is likely to spend based on demographics and behavior.

Suggested features:
- `Age`
- `Gender`
- `Country`
- `Signup_Date`
- `Email` / `Phone` pattern-derived features

All columns: `Customer_ID`, `Name`, `Age`, `Gender`, `Email`, `Phone`, `Country`, `Signup_Date`, `Purchase_Amount`. Values are intentionally messy: `Gender` mixes `M`, `F`, `Male`, `Female`, and blanks; 519 of the 1,000 `Age` values and 172 `Country` values are empty.

---

### 2) `sales_data.csv` — Sales Transactions
**Focus:** Outlier detection, numerical normalization, date/time handling, large-number transformations  
**Target:** `Is_Fraudulent`  
**Problem type:** Classification  
**Goal:** Identify whether a transaction is fraudulent.

Suggested features:
- `Transaction_Amount`
- `Payment_Method`
- `Discount_Applied`
- `Product_Category`
- `Transaction_Date`

---

### 3) `reviews_data.csv` — Product Reviews
**Focus:** Text preprocessing, sentiment analysis, categorical variables  
**Target:** `Sentiment`  
**Problem type:** Multiclass classification  
**Goal:** Classify reviews into positive, neutral, or negative sentiment.

Suggested features:
- `Review_Text`
- `Rating`
- `Review_Date`
- `Customer_ID`

---

### 4) `sensor_data.csv` — Sensor Readings
**Focus:** Time-series missing values, outliers, scaling  
**Target:** `Temperature` or `Humidity`  
**Problem type:** Regression  
**Goal:** Forecast sensor behavior using historical event patterns.

Suggested features:
- `Timestamp`
- `Humidity`
- `Pressure`
- Derived temporal features like hour, day, and month

---

### 5) `College.csv` — College Data
**Focus:** Institutional metrics, academic performance analysis  
**Problem type:** Classification / exploratory analysis  
**Goal:** Understand relationships between admission data and college outcomes.

Typical variables include:
- `Private`, `Apps`, `Accept`, `Enroll`
- `Top10perc`, `Top25perc`, `Outstate`
- `Room.Board`, `Books`, `Expend`, `Grad.Rate`

Other columns: `F.Undergrad`, `P.Undergrad`, `Personal`, `PhD`, `Terminal`, `S.F.Ratio`, `perc.alumni`. The first column has no header and contains the college name — load it with `index_col=0` in pandas.

---

### 6) `Iris.csv` — Iris Flower Dataset
**Focus:** Classic classification learning  
**Target:** `species`  
**Problem type:** Classification  
**Goal:** Predict the flower species using petal and sepal measurements.

Features:
- `sepal_length`
- `sepal_width`
- `petal_length`
- `petal_width`

---

### 7) `Purchase.csv` — Purchase Decision Dataset
**Focus:** Customer decision modeling  
**Target:** `Purchased`  
**Problem type:** Classification  
**Goal:** Predict whether a customer purchases based on their profile.

Columns:
- `Employee`
- `Age`
- `Salary`
- `Purchased` (target)

This file has only 10 rows, so it suits quick demonstrations rather than model evaluation.

---

### 8) `Salary.csv` — Experience vs Salary
**Focus:** Simple supervised learning  
**Target:** `salary`  
**Problem type:** Regression  
**Goal:** Estimate salary based on years of experience.

Features:
- `years_experience`
- `salary`

---

### 9) `Titanic.csv` — Titanic Survival Dataset
**Focus:** Data cleaning, feature engineering, survival analysis  
**Target:** `Survived`  
**Problem type:** Classification  
**Goal:** Predict passenger survival probability using profile and travel information.

Key variables include:
- `Pclass`, `Sex`, `Age`, `Fare`
- `SibSp`, `Parch`, `Embarked`
- `Cabin`, `Ticket`

Also included: `PassengerId` and `Name`.

---

## 🚀 Suggested Use Cases

This repository is ideal for:

- Learning Python or R for data science
- Practicing `pandas`, `numpy`, and `scikit-learn`
- Building regression and classification pipelines
- Cleaning messy datasets and handling missing values
- Creating EDA notebooks and portfolio projects
- Exploring feature engineering ideas

---

## 🐍 Quick Start with pandas

Use Python with pandas installed in your active environment:

```bash
python -m pip install pandas
```

Load a dataset directly from GitHub without cloning the repository:

```python
import pandas as pd

base = "https://raw.githubusercontent.com/gcfernando/datasets/main/"

titanic = pd.read_csv(base + "Titanic.csv")
college = pd.read_csv(base + "College.csv", index_col=0)  # first column = college name

print(titanic.shape)          # (891, 12)
print(titanic.isna().sum())   # missing values per column
```

Or clone the repository and read the files locally:

```bash
git clone https://github.com/gcfernando/datasets.git
cd datasets
```

From that folder, load the local CSV files:

```python
import pandas as pd

titanic = pd.read_csv("Titanic.csv")
college = pd.read_csv("College.csv", index_col=0)
print(titanic.shape)  # (891, 12)
```

---

## 🛠️ Recommended Learning Flow

1. Start with EDA
2. Clean missing values and inconsistent entries
3. Encode categorical variables
4. Engineer useful features
5. Train baseline models
6. Compare results and iterate

---

## ✅ Summary

This dataset collection is a compact, practical toolbox for machine learning and data analysis learning. It combines beginner-friendly datasets with more realistic business and time-series challenges, making it a great resource for students, researchers, and aspiring data scientists.

## ❓ FAQ

**Are the customer, sales, review, and sensor datasets real data?**
They appear to be synthetic: for example, customer IDs are random UUIDs and the email domains look generated. Treat them as practice data, not as real people or real business results.

**Which dataset should a beginner start with?**
`Iris.csv` for classification and `Salary.csv` for linear regression are small and clean. Move on to `Titanic.csv` for missing-value handling, then `customer_data.csv` and `sales_data.csv` for messier, more realistic cleaning.

<a id="source-and-reuse-notes"></a>

### Source and reuse notes

**Where did the classic datasets come from?**
`Iris.csv`, `Titanic.csv`, and `College.csv` are versions of widely used public teaching datasets. No source or license information is recorded in this repository, so check the original sources before redistributing them.

## 🔗 Related Projects

- [Salary prediction with scikit-learn](https://github.com/gcfernando/python_codes/blob/main/ML/Salary/readme.md) — uses the same `years_experience` / `salary` data
- [Python machine-learning examples](https://github.com/gcfernando/python_codes/tree/main/ML) — ARIMA forecasting and linear regression
- [Complete SQL guide](https://github.com/gcfernando/document/blob/main/sql_complete_guide.md) — load these CSV files into a database for SQL practice

---

## Documentation links

[Read all Machine Learning Practice Datasets guides online](https://gcfernando.github.io/datasets/documentation/) · [Project overview](https://gcfernando.github.io/datasets/) · [All developer projects](https://gcfernando.github.io/gcfernando/projects/)
