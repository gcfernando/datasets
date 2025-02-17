# customer_data.csv
## Customer Data (Missing values, duplicates, inconsistent data, categorical encoding, text cleaning)
🎯 Target: Purchase_Amount

Problem Type: Regression
Goal: Predict how much a customer is likely to spend based on their demographics and behavior.
Features to use: Age, Gender, Country, Signup Date, etc.

# sales_data.csv
## Sales Transactions (Outlier detection, numerical normalization, date/time handling, large number transformations)
🎯 Target: Is_Fraudulent (0 or 1)

Problem Type: Classification
Goal: Detect fraudulent transactions.
Features to use: Transaction Amount, Payment Method, Discount Applied, Product Category, etc.

# reviews_data.csv
## Product Reviews (Text preprocessing, sentiment analysis, categorical variables)
Problem Type: Classification (Multiclass)
Goal: Classify customer reviews into positive, neutral, or negative sentiment.
Features to use: Review Text (after text cleaning & vectorization), Rating, Review Date, etc.

# sensor_data.csv
## Sensor Readings (Time-series missing values, outliers, scaling)
🎯 Target: Temperature (or Humidity)

Problem Type: Regression
Goal: Predict temperature/humidity levels based on past sensor readings.
Features to use: Timestamp (converted into features like Hour, Day, Month), Humidity, Pressure, etc.