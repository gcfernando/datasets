# 🌟 Dataset Playground

Welcome to the repository of ready-to-use datasets for machine learning, data cleaning, feature engineering, and exploratory analysis. This collection includes tabular, classification, regression, and time-series datasets designed for both learning and experimentation.

## ✨ What’s inside?

This repo contains 9 structured datasets across common ML scenarios:

- Customer behavior and spend prediction
- Fraud detection
- Sentiment analysis
- Time-series forecasting
- Classic ML benchmark datasets
- Real-world business and academic examples

---

## 📊 Dataset Catalog

| File | Theme | Problem Type | Target/Goal | Best For |
|---|---|---:|---|---|
| `customer_data.csv` | Customer analytics | Regression | Predict `Purchase_Amount` | EDA, data cleaning, feature engineering |
| `sales_data.csv` | Transactions | Classification | Detect `Is_Fraudulent` | Fraud detection, anomaly handling |
| `reviews_data.csv` | Product feedback | Multiclass classification | Predict review sentiment | NLP, text preprocessing |
| `sensor_data.csv` | IoT sensor readings | Regression | Predict `Temperature` / `Humidity` | Time-series modeling, missing data handling |
| `College.csv` | Higher education | Classification | Predict college outcomes / categories | Feature selection, logistic regression |
| `Iris.csv` | Botanical dataset | Classification | Identify flower species | Beginner ML, clustering, classification |
| `Purchase.csv` | Customer purchase behavior | Classification | Predict purchase decision | Marketing analytics |
| `Salary.csv` | Employment dataset | Regression | Predict salary from experience | Linear regression, simple modeling |
| `Titanic.csv` | Passenger data | Classification | Predict survival | Data wrangling, binary classification |

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

Typical features:
- `Employee`
- `Age`
- `Salary`
- `Purchased`

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

If you want, you can also turn this into a more polished project homepage with:
- a cover image banner
- dataset badges
- sample notebook links
- usage examples in Python
- project roadmap or learning path
